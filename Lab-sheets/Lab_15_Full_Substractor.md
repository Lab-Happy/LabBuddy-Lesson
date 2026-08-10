### **Lab 15: Full Subtractor (วงจบลบเลขดิจิทัล 1 บิตสมบูรณ์)** — คำนวณผลต่าง ($Difference$) และตัวยืม ($Borrow$) ด้วย 3 อินพุต

#### 15.1 **Cover Page**
**File name:** Lab_15_Full_Substractor_circuit_Lesson
**Title:** Full Subtractor Lesson
**Subtitle:** วงจบลบเลขฐานสอง 1 บิตสมบูรณ์
**IC Label:** 7486 / 7404 / 7408 / 7432

**Objectives:**
- เข้าใจการลบเลขฐานสองที่มีตัวยืมเข้า ($B_{IN}$)
- สร้างวงจร Full Subtractor จาก Half Subtractor 2 ชุดและ OR Gate 1 ตัว
- ทดสอบผลต่าง ($DIFF$) และตัวยืมออก ($BORROW$) ครบทั้ง 8 สภาวะตรรกะ

#### 15.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Full Subtractor รับอินพุต 3 ช่อง ($A, B, B_{IN}$) เพื่อคำนวณผลลบสมบูรณ์ ($A - B - B_{IN}$):
- **Difference ($DIFF$):** $D = A \oplus B \oplus B_{IN}$
- **Borrow Out ($BORROW$):** $B_{OUT} = \overline{A} \cdot B + \overline{(A \oplus B)} \cdot B_{IN}$

#### 15.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบด้วย XOR Gate 2 ตัว, NOT Gate 2 ตัว, AND Gate 2 ตัว และ OR Gate 1 ตัว
**Inputs:** A, B, B_IN
**Outputs:** DIFF, BORROW
**Gate Type:** XOR, NOT, AND, OR

**Body (optional):** ต่อเอาต์พุต Difference ของ Half Subtractor ชุดแรกเข้าเป็นอินพุตของ Half Subtractor ชุดที่สองร่วมกับ B_IN จากนั้นนำสัญญาณ Borrow Out ของ Half Subtractor ทั้งสองชุดมาผ่าน OR Gate เพื่อสร้างเอาต์พุต BORROW สมบูรณ์

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_15_Full_Substractor_circuit.drawio.svg)

#### 15.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7486, 7404, 7408, 7432
**Instructions:**
- ทดสอบป้อนสภาวะอินพุตทั้ง 8 สภาวะ ($2^3 = 8$)
- ตรวจสอบเอาต์พุต DIFF และ BORROW ตามการคำนวณ $A - B - B_{IN}$

**Verification Text:** ตรวจสอบวงจร Full Subtractor ครบทั้ง 8 สภาวะตรรกะ

**Truth Table:**
- A=0, B=0, B_IN=0 --> DIFF=0, BORROW=0
- A=0, B=0, B_IN=1 --> DIFF=1, BORROW=1
- A=0, B=1, B_IN=0 --> DIFF=1, BORROW=1
- A=0, B=1, B_IN=1 --> DIFF=0, BORROW=1
- A=1, B=0, B_IN=0 --> DIFF=1, BORROW=0
- A=1, B=0, B_IN=1 --> DIFF=0, BORROW=0
- A=1, B=1, B_IN=0 --> DIFF=0, BORROW=0
- A=1, B=1, B_IN=1 --> DIFF=1, BORROW=1

#### 15.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจโครงสร้างและสามารถสร้างวงจร Full Subtractor สำหรับใช้ลบเลขหลายบิตได้อย่างถูกต้อง
