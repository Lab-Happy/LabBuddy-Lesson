
### **Lab 06: Sum of Products (SOP) Circuit** — วงจรตรรกะจากสมการมินเทอม (AND-OR Logic)

#### 6.1 **Cover Page**
**File name:** Lab_06_Sum_Of_Product_circuit_Lesson
**Title:** Sum of Products (SOP) Lesson
**Subtitle:** การสร้างวงจรตรรกะจากสมการมินเทอม
**IC Label:** 7404 / 7408 / 7432

**Objectives:**
- เรียนรู้การแปลงสมการบูลีนรูปแบบ Sum of Products (SOP) เป็นวงจรเกตตรรกะ
- สามารถสร้างวงจรโครงสร้าง AND-OR Logic
- สามารถทดสอบผลลัพธ์ตรรกะผสม 2-3 อินพุต

#### 6.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** รูปแบบ Sum of Products (SOP) คือการนำมินเทอมที่เกิดจากการคูณ (AND) มารวมกันด้วยการบวก (OR) เช่น $Y = A \cdot B + \overline{A} \cdot \overline{B}$ ซึ่งทำหน้าที่เป็นวงจรตรวจสอบความเหมือน

#### 6.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ NOT Gate 2 ตัว, AND Gate 2 ตัว และ OR Gate 1 ตัว
**Inputs:** A, B
**Outputs:** Y
**Gate Type:** NOT, AND, OR

**Body (optional):** สร้างวงจร $Y = A \cdot B + \overline{A} \cdot \overline{B}$ โดยลากสายสัญญาณจากอินพุต A, B และสายสัญญาณที่ผ่าน NOT Gate เข้าไปยัง AND Gate แล้วนำเอาต์พุตมารวมกันที่ OR Gate


![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_06_SOP_circuit.drawio.svg)

#### 6.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7404, 7408, 7432
**Instructions:**
- ตรวจสอบจุดเชื่อมต่อสายสัญญาณ Junction ให้ถูกต้อง
- ป้อนสภาวะอินพุต 00, 01, 10, 11 แล้วสังเกตเอาต์พุต Y

**Verification Text:** ตรวจสอบว่าเอาต์พุต Y เป็น 1 เมื่ออินพุตทั้งสองเหมือนกัน (00 หรือ 11)

**Truth Table:**
- A=0, B=0 --> Y=1
- A=0, B=1 --> Y=0
- A=1, B=0 --> Y=0
- A=1, B=1 --> Y=1

#### 6.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนสามารถออกแบบและสร้างวงจรตรรกะผสมรูปแบบ Sum of Products (SOP) ได้สำเร็จ