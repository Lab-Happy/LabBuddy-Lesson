### **Lab 09: Universal Gate Construction** — สร้าง AND จาก NAND Gate

https://www.geeksforgeeks.org/digital-logic/basic-conversion-of-logic-gates/

#### 9.1 **Cover Page**
**File name:** Lab_09_And_from_nand_circuit_Lesson
**Title:** Universal Gate Construction Lesson
**Subtitle:** การสร้าง AND Gate จาก NAND Gate
**IC Label:** 7400

**Objectives:**
- พิสูจน์คุณสมบัติ Universal Gate ของ NAND Gate
- สามารถต่อ NAND Gate ดัดแปลงเป็น AND Gate
- ฝึกทักษะการลดจำนวนชนิดไอซีในงานออกแบบฮาร์ดแวร์

#### 9.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** NAND Gate เป็น Universal Gate ที่สามารถสร้างเกตตรรกะอื่นได้ทั้งหมด โดยการกลับสัญญาณเอาต์พุตของ NAND Gate ด้วย NOT Gate (NAND รวบขา):
1. **NOT:** รวบขาอินพุต NAND เข้าด้วยกัน ($\overline{A \cdot A} = \overline{A}$)
2. **AND:** ต่อ NOT หลัง NAND Gate ($\overline{\overline{A \cdot B}} = A \cdot B$)
3. **OR:** ใช้ NOT ที่อินพุตแต่ละขาก่อนเข้า NAND Gate ($\overline{\overline{A} \cdot \overline{B}} = A + B$)

#### 9.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ IC 7400 ประกอบเป็นวงจร AND Gate จาก NAND 2 ตัว
**Inputs:** A, B
**Outputs:** Y_AND
**Gate Type:** NAND

**Body (optional):** ต่อ NAND ตัวที่ 1 รับสัญญาณอินพุต $A$ และ $B$ เพื่อทำหน้าที่เป็น NAND Gate ($\overline{A \cdot B}$) จากนั้นนำเอาต์พุตเข้า NAND ตัวที่ 2 ซึ่งรวบขาอินพุตทำหน้าที่เป็น NOT Gate เพื่อให้ได้ผลลัพธ์เป็น $\overline{\overline{A \cdot B}} = A \cdot B$

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_09_And_from_nand_Circuit.drawio.svg)

#### 9.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7400
**Instructions:**
- ต่อ NAND Gate 2 ตัวบน IC 7400 ตามไดอะแกรม
- ป้อนอินพุต A, B ตรวจสอบว่าผลลัพธ์ตรงกับฟังก์ชัน AND Gate หรือไม่

**Verification Text:** ตรวจสอบว่าวงจรที่สร้างด้วย NAND Gate 2 ตัวให้ผลลัพธ์เหมือน AND Gate 100%

**Truth Table:**
- A=0, B=0 --> Y_AND=0
- A=0, B=1 --> Y_AND=0
- A=1, B=0 --> Y_AND=0
- A=1, B=1 --> Y_AND=1

#### 9.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนพิสูจน์ได้ว่า NAND Gate 2 ตัวสามารถนำมาต่อรวมกันเพื่อสร้างฟังก์ชัน AND Gate ได้สำเร็จ