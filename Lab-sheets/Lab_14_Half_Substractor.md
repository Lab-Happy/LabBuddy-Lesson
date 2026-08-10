### **Lab 14: Half Subtractor (วงจบลบเลขดิจิทัล)** — คำนวณผลต่าง ($Difference$) และตัวยืม ($Borrow$)

#### 14.1 **Cover Page**
**File name:** Lab_14_Half_Substractor_circuit_Lesson
**Title:** Half Subtractor Lesson
**Subtitle:** วงจบลบเลขฐานสองขนาดครึ่งบิต
**IC Label:** 7486 / 7404 / 7408

**Objectives:**
- เข้าใจหลักการลบเลขฐานสอง ($A - B$)
- สร้างวงจร Half Subtractor คำนวณค่า Difference ($D$) และ Borrow Out ($B_{OUT}$)
- เรียนรู้ความสัมพันธ์ระหว่างวงจรบวกและวงจบลบเลขดิจิทัล

#### 14.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Half Subtractor ทำหน้าที่ลบเลข 1 บิต ($A - B$):
- **Difference ($D$):** $D = A \oplus B$
- **Borrow Out ($B_{OUT}$):** $B_{OUT} = \overline{A} \cdot B$ (ต้องยืมเมื่อ $A=0$ และ $B=1$)

#### 14.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ XOR Gate 1 ตัวสำหรับ Difference และ NOT + AND Gate สำหรับ Borrow Out
**Inputs:** A, B
**Outputs:** DIFF, BORROW
**Gate Type:** XOR, NOT, AND

**Body (optional):** อินพุต A ถูกกลับค่าด้วย NOT Gate ก่อนนำไป AND กับอินพุต B เพื่อสร้างสัญญาณตัวยืม BORROW

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_14_Half_Substractor_circuit.drawio.svg)

#### 14.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7486, 7404, 7408
**Instructions:**
- ป้อนสภาวะอินพุต $0-0, 0-1, 1-0, 1-1$
- ตรวจสอบเอาต์พุต DIFF และ BORROW

**Verification Text:** ตรวจสอบการลบเลขฐานสอง โดยเฉพาะสภาวะ $0 - 1 = 1$ (ยืม 1)

**Truth Table:**
- A=0, B=0 --> DIFF=0, BORROW=0
- A=0, B=1 --> DIFF=1, BORROW=1
- A=1, B=0 --> DIFF=1, BORROW=0
- A=1, B=1 --> DIFF=0, BORROW=0

#### 14.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจหลักการลบเลขฐานสองระดับบิตพื้นฐานด้วย Half Subtractor เรียบร้อยแล้ว