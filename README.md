# Kafka Origin Whisper (`W1.0.3`)

> เอกสารฉบับนี้มีทั้งภาษาไทยและภาษาอังกฤษ / This document is written in Thai first, followed by English.

---

## ภาษาไทย (Thai)

### Whisper คืออะไร?

**Whisper** คือแพตช์ตัวเกมและตัววัดดาเมจในเกมของชุด **Kafka Origin** สำหรับเกม **Zenless Zone Zero** โดยทำงานร่วมกับลันเชอร์ (Script) และเซิร์ฟเวอร์ (Hunter):

- **`kafka.exe` และ `kafka.dll`** — เปิดตัวเกมพร้อมเชื่อมต่อกับเซิร์ฟเวอร์ส่วนตัว โหลดค่า `offsets.zon` และแสดงข้อความบนหน้าจอ (`custom.uid`)
- **`kafka-meter.dll`** — ตัววัดดาเมจสไตล์ Veritas ภายในเกม แสดงดาเมจรวม ดาเมจและสัดส่วนของแต่ละเอเจนต์ (DPS, DPS เฉลี่ย 5 วินาที, DPS สูงสุด, จำนวนฮิต และเวลาต่อสู้) รองรับทั้งภาษาไทยและภาษาอังกฤษ (คีย์ลัด: `Ctrl+M` เปิดเมนูตั้งค่า/รีเซ็ต/คัดลอกสรุป/บันทึก PNG, `Ctrl+H` ซ่อนหรือแสดงแผง, `Ctrl+F8` เปิด/ปิด, `\` แยกหน้าต่างลอย)
  - ในเวอร์ชัน **`W1.0.3`** ตัววัดดาเมจทำงานบนตัวเกม `3.4.5` ได้อย่างสมบูรณ์ แผงตัววัดดาเมจจะแสดงระหว่างการต่อสู้ และซ่อนตัวเองภายในไม่กี่วินาทีหลังจากออกจากการต่อสู้ (ก่อนหน้านี้ แผงอาจค้างพร้อมตัวเลขเดิมเมื่ออยู่ในเมืองหลังจบการต่อสู้ครั้งแรก) และใช้ CPU น้อยมากก่อนเริ่มการต่อสู้ครั้งแรก

ซอร์สโค้ดเป็นแบบส่วนตัวและไม่มีการเผยแพร่ คลังสาธารณะนี้เก็บเฉพาะหน้า README และไฟล์รีลีสที่ลงลายเซ็นแล้วเท่านั้น

### เวอร์ชัน

- **Whisper:** `W1.0.3` (อยู่ในชุด **Kafka Origin `K2.0.0`** ร่วมกับ Script `S2.0.0` และ Hunter `H2.0.0`)
- **ตัวเกมที่รองรับ:** `CNBetaWin3.4.5` (`W1.0.3 · เกม 3.4.5`)

### ไฟล์รีลีสอยู่ที่ไหน?

ไฟล์รีลีสที่ลงลายเซ็นแล้ว (`kafka-origin-whisper-W1.0.3.zip`, `SHA256SUMS` และ `SHA256SUMS.sig`) เผยแพร่อยู่ที่หน้า [Releases ของ xaoxz/Kafka-Origin-Whisper](https://github.com/xaoxz/Kafka-Origin-Whisper/releases)

### วิธีติดตั้ง

**ติดตั้งผ่านตัวติดตั้ง Kafka Origin** จากคลังหลัก [xaoxz/Kafka-Origin](https://github.com/xaoxz/Kafka-Origin/releases/latest):

- **Windows:** ดาวน์โหลด `KafkaOrigin-Setup.exe` หรือ `KafkaOrigin-Setup-Offline.exe`
- **Linux:** รันคำสั่ง:
  ```bash
  curl -fsSL https://github.com/xaoxz/Kafka-Origin/releases/latest/download/install.sh | bash
  ```

ลันเชอร์ **Script** จะติดตั้ง ตรวจสอบลายเซ็น และอัปเดต Whisper ให้โดยอัตโนมัติผ่านหน้า **Updates** โดยไม่ต้องแตกไฟล์วางเอง

---

## English

### What is Whisper?

**Whisper** is the client patch and in-game damage meter of **Kafka Origin** for **Zenless Zone Zero**, built to work alongside the launcher (Script) and server (Hunter):

- **`kafka.exe` and `kafka.dll`** — start the game client connected to your local server, load `offsets.zon`, and draw customizable on-screen HUD text (`custom.uid`).
- **`kafka-meter.dll`** — draws a Veritas-style in-game damage meter showing total damage, per-agent rows (portrait, name, damage, share bar, DPS), 5-second DPS, peak DPS, hit counts, and the battle clock in Thai or English (`Ctrl+M` opens the menu to reset, copy summary, or export PNG; `Ctrl+H` hides/shows the panel; `Ctrl+F8` toggles it on/off; `\` floats it on its own window).
  - In **`W1.0.3`**, the damage meter works on game `3.4.5`; its panel shows during a fight and hides within a few seconds after you leave the fight (before, the panel could stay up with old numbers in the city after the first fight), and before the first fight it uses little CPU.

Source code is private and never published; this public repository holds only this README and signed release files.

### Version

- **Whisper:** `W1.0.3` (part of **Kafka Origin `K2.0.0`** with Script `S2.0.0` and Hunter `H2.0.0`)
- **Game version:** `CNBetaWin3.4.5` (`W1.0.3 · game 3.4.5`)

### Where Releases Are

Signed release archives (`kafka-origin-whisper-W1.0.3.zip`, `SHA256SUMS`, and `SHA256SUMS.sig`) are published on [xaoxz/Kafka-Origin-Whisper Releases](https://github.com/xaoxz/Kafka-Origin-Whisper/releases).

### How to Install

**Install through Kafka Origin Setup** from [xaoxz/Kafka-Origin](https://github.com/xaoxz/Kafka-Origin/releases/latest):

- **Windows:** Download and run `KafkaOrigin-Setup.exe` (online) or `KafkaOrigin-Setup-Offline.exe` (offline).
- **Linux:** Run:
  ```bash
  curl -fsSL https://github.com/xaoxz/Kafka-Origin/releases/latest/download/install.sh | bash
  ```

The **Script** launcher deploys, verifies, and updates Whisper automatically through its **Updates** page — no manual unpacking required.
