### **Lab 01: NOT Gate (Inverter)** — การทำงานของ Inverter และสวิตช์อินพุต

#### 1.1 **Cover Page**
**File name:** Lab_01_Not_Gate_circuit_Lesson
**Title:** NOT Gate Lesson
**Subtitle:** การทดลอง NOT Gate
**IC Label:** 7404

**Objectives:**
- เข้าใจหลักการทำงานของ NOT Gate
- สามารถสร้างวงจรอินเวอร์เตอร์
- สามารถทดสอบผลลัพธ์ด้วยตารางความจริง

#### 1.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** NOT Gate หรือ Inverter เป็นลอจิกเกตที่ทำหน้าที่กลับค่าของอินพุต ถ้าอินพุตเป็น 1 ผลลัพธ์จะเป็น 0 ถ้าอินพุตเป็น 0 ผลลัพธ์จะเป็น 1

#### 1.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ต่อสายบน protoboard
**Inputs:** A
**Outputs:** Y
**Gate Type:** NOT

**Body (optional):** วงจรอินเวอร์เตอร์สามารถสร้างได้โดยใช้ IC 7404 ซึ่งมี NOT Gate อยู่ภายใน เลือกใช้หนึ่งช่องของ IC แล้วต่ออินพุตเข้าขา A และต่อเอาต์พุต Y ออกไปยัง LED


![](100-Projects/103-LabBuddy/08_Labsheet/Lab_01_Not_Gate/Lab_01_Not_Gate_circuit.drawio.svg)

#### 1.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7404
**Instructions:**
- ต่อวงจร
- ตรวจสอบวงจร

**Verification Text:** การตรวจสอบวงจรอินเวอร์เตอร์จะใช้ตารางความจริงของ NOT Gate โดยป้อนค่าอินพุต 0 และ 1 แล้วตรวจสอบว่าเอาต์พุตกลับค่าถูกต้อง

**Truth Table:**
- A=0 --> Y=1
- A=1 --> Y=0

#### 1.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ ผู้เรียนสามารถเข้าใจหลักการทำงานของ NOT Gate และทดสอบวงจรอินเวอร์เตอร์ได้อย่างถูกต้อง