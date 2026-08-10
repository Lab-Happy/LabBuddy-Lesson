
### **Lab 08: Universal Gate Construction** — สร้าง NOT จาก NAND Gate 

https://www.geeksforgeeks.org/digital-logic/basic-conversion-of-logic-gates/

#### 8.1 **Cover Page**
**File name:** Lab_08_Not_from_nand_circuit_Lesson
**Title:** Universal Gate Construction Lesson
**Subtitle:** การสร้าง NOT ด้วย NAND Gate
**IC Label:** 7400

**Objectives:**
- พิสูจน์คุณสมบัติ Universal Gate ของ NAND Gate
- สามารถต่อ NAND Gate ดัดแปลงเป็น NOT, AND และ OR Gate
- ฝึกทักษะการลดจำนวนชนิดไอซีในงานออกแบบฮาร์ดแวร์

#### 8.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** NAND Gate เพียงชนิดเดียวสามารถนำมาต่อรวมกันเพื่อแทนเกตอื่นได้ทั้งหมด:
1. **NOT:** รวบขาอินพุต NAND เข้าด้วยกัน ($\overline{A \cdot A} = \overline{A}$)
2. **AND:** ต่อ NOT (NAND รวบขา) หลัง NAND Gate ($\overline{\overline{A \cdot B}} = A \cdot B$)
3. **OR:** ใส่ NOT ที่อินพุตแต่ละขาก่อนเข้า NAND ($\overline{\overline{A} \cdot \overline{B}} = A + B$)

#### 8.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ IC 7400 ประกอบเป็นวงจร NOT Gate จาก NAND 1 ตัว โดยการรวบขาอินพุตเข้าด้วยกัน
**Inputs:** A
**Outputs:** Y
**Gate Type:** NAND

**Body (optional):** ต่อ NAND Gate โดยรวบขาอินพุตทั้งสองเข้าด้วยกันเพื่อรับสัญญาณอินพุต $A$ เดียวกัน จะทำให้ได้ผลลัพธ์ทางเอาต์พุตเป็น $Y = \overline{A \cdot A} = \overline{A}$ ซึ่งทำหน้าที่เป็น NOT Gate

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_08_not_from_nand_Circuit.drawio.svg)

#### 8.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7400
**Instructions:**
- ต่อ NAND Gate 1 ตัวบน IC 7400 โดยรวบขาอินพุตเข้าด้วยกันตามไดอะแกรม
- ป้อนอินพุต A ตรวจสอบว่าผลลัพธ์ตรงกับฟังก์ชัน NOT Gate หรือไม่

**Verification Text:** ตรวจสอบว่าวงจรที่สร้างด้วย NAND Gate 1 ตัว (รวบขาอินพุต) ให้ผลลัพธ์เหมือน NOT Gate 100%

**Truth Table:**
- A=0 --> Y=1
- A=1 --> Y=0

#### 8.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนพิสูจน์ได้ว่า NAND Gate สามารถนำมารวบขาอินพุตเพื่อสร้างฟังก์ชัน NOT Gate ได้สำเร็จ