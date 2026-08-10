### **Lab 13: Full Adder (วงจรบวกเลข 1 บิตสมบูรณ์)** — วงจรบวก 3 อินพุต ($A, B, C_{IN}$) ด้วย 5 ลอจิกเกต

#### 13.1 **Cover Page**
**File name:** Lab_13_Full_Adder_circuit_Lesson
**Title:** Full Adder Lesson
**Subtitle:** วงจรบวกเลขฐานสอง 1 บิตสมบูรณ์
**IC Label:** 7486 / 7408 / 7432

**Objectives:**
- เข้าใจการบวกเลขฐานสองที่มีตัวนำเข้า ($C_{IN}$)
- สร้างวงจร Full Adder จาก Half Adder 2 ชุดและ OR Gate 1 ตัว
- ทดสอบการบวกเลขแบบมีตัวนำเข้าและตัวนำออก

#### 13.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Full Adder รับอินพุต 3 ช่อง ($A, B, C_{IN}$) เพื่อคำนวณผลบวกสมบูรณ์:
- **SUM ($S$):** $S = A \oplus B \oplus C_{IN}$
- **Carry Out ($C_{OUT}$):** $C_{OUT} = (A \oplus B) \cdot C_{IN} + A \cdot B$

#### 13.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบด้วย XOR 2 ตัว, AND 2 ตัว และ OR 1 ตัว (รวม 5 เกต)
**Inputs:** A, B, C_IN
**Outputs:** SUM, C_OUT
**Gate Type:** XOR, AND, OR

**Body (optional):** ต่อเอาต์พุต SUM ของ Half Adder ชุดแรกเข้าเป็นอินพุตของ Half Adder ชุดที่สองร่วมกับ C_IN จากนั้นรวมสัญญาณ Carry-Out ของ Half Adder ทั้งสองชุดด้วย OR Gate

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_13_Full_Adder_circuit.drawio.svg)

#### 13.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7486, 7408, 7432
**Instructions:**
- ทดสอบป้อนสภาวะอินพุตทั้ง 8 สภาวะ ($2^3 = 8$)
- ยืนยันค่า SUM และ C_OUT ตามผลบวกเลขฐานสอง

**Verification Text:** ตรวจสอบวงจร Full Adder ครบทั้ง 8 สภาวะตรรกะ

**Truth Table:**
- A=0, B=0, C_IN=0 --> SUM=0, C_OUT=0
- A=0, B=0, C_IN=1 --> SUM=1, C_OUT=0
- A=0, B=1, C_IN=0 --> SUM=1, C_OUT=0
- A=0, B=1, C_IN=1 --> SUM=0, C_OUT=1
- A=1, B=0, C_IN=0 --> SUM=1, C_OUT=0
- A=1, B=0, C_IN=1 --> SUM=0, C_OUT=1
- A=1, B=1, C_IN=0 --> SUM=0, C_OUT=1
- A=1, B=1, C_IN=1 --> SUM=1, C_OUT=1

#### 13.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจโครงสร้างและสามารถสร้างวงจร Full Adder สำหรับใช้บวกเลขหลายบิตได้สำเร็จ
