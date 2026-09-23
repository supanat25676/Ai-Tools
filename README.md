# 🤖 AI Experiments & Financial Analytics Project

โปรเจกต์สรุปการทดลองใช้งาน AI Models, การประมวลผลและทำความสะอาดข้อมูล (Data Cleaning & Merging Pipeline) และการพัฒนาแอปพลิเคชันช่วยคำนวณความเสี่ยงการลงทุนในตลาดทองคำ (XAU/USD)

📄 **[คลิกเพื่อดูเอกสารนำเสนอฉบับเต็ม (PDF)](./การตัดสิน%20AI%20(1)_compressed.pdf)**

---

## 📌 Highlight Projects

### 1. 🥇 XAU Power - Gold Investment & Risk Management App
แอปพลิเคชันพัฒนาผ่าน **Google AI Studio** ช่วยวิเคราะห์ตลาดและคำนวณ Money Management สำหรับการเทรดทองคำ (XAU/USD) เพื่อลดอารมณ์และเพิ่มความแม่นยำในการตัดสินใจ
* **Features:**
  * คำนวณ Lot Size อัตโนมัติจาก Account Balance, % Risk Per Trade และ Leverage (เช่น 1:200)
  * วิเคราะห์โครงสร้างตลาด (Market Trend / Sideway Up) และสภาวะตลาดแบบ Real-time
  * AI Assistant คอยตอบข้อสงสัยเกี่ยวกับการลงทุน
* **Future Roadmap:** เพิ่มระบบคำนวณจุดเข้าซื้อ (Entry Point) และจุดตัดขาดทุน (Stop Loss / Take Profit) บนกราฟโดยตรง

---

### 2. 🧹 Data Cleaning & Merging Pipeline
กระบวนการทำความสะอาดและรวมชุดข้อมูล (Data Cleaning & Merging Rules) ระหว่างข้อมูลการใช้งาน Social Media กับพฤติกรรมเชิงลึก
* **Data Cleaning Rules:**
  * **Text to Numeric:** เปลี่ยนค่าข้อความ เช่น `"twenty"` ➔ `20.0`
  * **Typo Correction:** แก้ไขคำที่พิมพ์ผิด เช่น `"mal"` ➔ `"Male"`, `"femail"` ➔ `"Female"`
  * **Standardization:** ปรับรูปแบบตัวอักษร เช่น `"master"` ➔ `"Master"`
  * **Missing Values (NaNs):** แปลงคำว่า `"missing"` และช่องว่างเป็น NaN แล้วแทนที่ด้วย ค่ามัธยฐาน (Median) สำหรับข้อมูลตัวเลข และ ค่าฐานนิยม (Mode) สำหรับข้อมูลตัวอักษร
* **Data Merging:** เชื่อมตารางข้อมูล (Inner Join) ด้วยตัวแปรประชากรศาสตร์ (`Age`, `Gender`) เพื่อศึกษาความสัมพันธ์ระหว่างระยะเวลาที่ใช้บนแพลตฟอร์มกับระดับภาวะอารมณ์/ความเครียด (Depression Score)

---

### 3. 🧪 AI Model Comparison (OpenRouter API)
การทดสอบและเปรียบเทียบคำตอบจาก AI Models ต่างๆ ผ่าน OpenRouter API:
| Model Name | คุณลักษณะและจุดเด่น |
| :--- | :--- |
| **NVIDIA: Nemotron 3.5 Lightning** | สรุปอ่านง่าย มีการใช้สัญลักษณ์ Visual ช่วยดึงสายตา เสนอแนวทางเจาะจงในการศึกษาต่อได้ดี |
| **Poolside: Laguna S 2.1** | เหมาะกับคนที่ชอบเนื้อหาเรียบๆ มีโครงสร้างหัวข้อชัดเจนแบบตำราเรียน |

---

## 🛠️ Tech Stack & Tools
* **AI & Cloud Platform:** Google AI Studio, OpenRouter API
* **AI Models:** NVIDIA Nemotron 3.5 Lightning, Poolside Laguna S 2.1
* **Data Processing:** Python, Data Cleaning & Preprocessing Techniques
* **Asset Class:** Forex / Gold (XAU/USD)
