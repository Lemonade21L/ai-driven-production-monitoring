# VisionFlow: AI-Driven Production Monitoring System

## 🚀 Project Overview
**VisionFlow** is an industrial AI solution designed to verify real-time production status. By utilizing Computer Vision (CCTV) and Deep Learning, the system detects actual products on a conveyor belt to ensure the machine is actively producing, rather than just being powered on.

## ⚠️ Problem Statement
In many manufacturing plants, **Tower Lamps** only indicate electrical power status (Green = Power On). This creates a "False Green" situation where the lamp is green, but the conveyor is empty or stalled, leading to inaccurate OEE (Overall Equipment Effectiveness) data.

## 💡 Solution
We bridge this gap by using AI to detect the physical presence of products. If a product is detected on the moving conveyor, the system triggers a **"True Running"** status to the database via API.

## 🏗️ Workflow & Architecture
1. **Visual Input:** Connect CCTV stream with **CiraCore AI**.
2. **Deep Detection:** AI model identifies products on the conveyor.
3. **Logic Processing:** JavaScript script processes the detection value (Detected = Running).
4. **Data Transmission:** Send JSON payloads using **RestPutJson** module.
5. **Integration:** Update the central database via API end-points.

## 🎨 Design & Compliance
> [!NOTE]
> **Policy Compliance:** To comply with corporate NDA and privacy policies, actual factory footage and confidential source codes have been abstracted. System visuals are presented as high-fidelity **engineering sketches** created on iPad/Procreate and flowcharts via **Draw.io** to demonstrate the system logic.

## 🛠️ Technology Stack
- **AI Engine:** CiraCore (Deep Learning Engine)
- **Language:** Python Plus
- **Communication:** RESTful API (JSON)
- **Design Tools:** Procreate (for System Sketches), Draw.io (for Flowcharts & Diagrams)

## 🙏 Acknowledgements
Special thanks to the **CIRA Automation Team** for providing **CiraCore**, which serves as the core AI inference engine for this project.
- Website: [https://www.cira-ai.com/](https://www.cira-ai.com/)

## 📄 License
This project is licensed under the **MIT License**.

---

# VisionFlow: ระบบตรวจสอบสถานะการผลิตด้วย AI สำหรับงานอุตสาหกรรม

## 🚀 ภาพรวมโครงการ
**VisionFlow** คือโซลูชัน AI สำหรับอุตสาหกรรมที่ออกแบบมาเพื่อตรวจสอบสถานะการผลิตแบบเรียลไทม์ โดยใช้ Computer Vision (CCTV) และ Deep Learning ในการตรวจจับชิ้นงานจริงบนสายพาน เพื่อให้มั่นใจว่าเครื่องจักรกำลังผลิตงานอยู่จริง ไม่ใช่เพียงแค่เปิดเครื่องทิ้งไว้

## ⚠️ ปัญหาที่พบ
ในโรงงานอุตสาหกรรมหลายแห่ง **Tower Lamp** จะบอกเพียงสถานะไฟฟ้า (สีเขียว = เปิดเครื่อง) ซึ่งทำให้เกิดปัญหา "False Green" หรือสถานะเขียวหลอก คือไฟเขียวแต่สายพานว่างเปล่าหรือติดขัด ทำให้ข้อมูลประสิทธิภาพการผลิต (OEE) คลาดเคลื่อนจากความเป็นจริง

## 💡 วิธีการแก้ไข
เราแก้ไขปัญหานี้ด้วยการใช้ AI ตรวจจับการมีอยู่ของชิ้นงาน หากตรวจพบชิ้นงานบนสายพานที่กำลังเคลื่อนที่ ระบบจะส่งสถานะ **"True Running"** (กำลังผลิตจริง) เข้าสู่ฐานข้อมูลผ่าน API ทันที

## 🏗️ ขั้นตอนการทำงาน
1. **รับภาพ:** เชื่อมต่อกล้อง CCTV เข้ากับ **CiraCore AI**
2. **ตรวจจับ:** ใช้โมเดล Deep Learning ตรวจจับชิ้นงานบนสายพาน
3. **ประมวลผล:** ใช้ Python Plus ประมวลผลค่าที่ได้ (หากตรวจพบ = สถานะ Running)
4. **ส่งข้อมูล:** แปลงค่าเป็น JSON และส่งผ่านโมดูล **RestPutJson**
5. **บันทึกผล:** อัปเดตข้อมูลไปยัง API End-point ของระบบฐานข้อมูล

## 🎨 การออกแบบและนโยบายความเป็นส่วนตัว
> [!IMPORTANT]
> **การปฏิบัติตามนโยบาย:** เพื่อให้เป็นไปตามนโยบายรักษาความลับของบริษัท ภาพถ่ายจริงในโรงงานและซอร์สโค้ดบางส่วนถูกปิดบังไว้ โดยจะแสดงภาพรวมของระบบผ่าน **แบบร่างทางวิศวกรรม (Engineering Sketches)** ที่วาดด้วย iPad/Procreate และผังงานจาก **Draw.io** แทนเพื่อแสดงตรรกะการทำงานของระบบ

## 🛠️ เทคโนโลยีที่ใช้
- **AI Engine:** CiraCore (Deep Learning Engine)
- **Language:** Python Plus
- **Communication:** RESTful API (JSON)
- **Design Tools:** Procreate (สำหรับวาดภาพประกอบ), Draw.io (สำหรับเขียน Flowchart)

## 🙏 กิตติกรรมประกาศ
ขอขอบคุณทีมผู้พัฒนา **CIRA Automation** สำหรับเครื่องมือ **CiraCore** ที่ใช้เป็นหัวใจหลักในการประมวลผล AI ในโครงการนี้
- เว็บไซต์: [https://www.cira-ai.com/](https://www.cira-ai.com/)
