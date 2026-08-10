### **Lab 12: NAND Gate Half Adder (วงจรบวกเลขครึ่งบิตด้วย NAND Gate)**

#### 12.1 **Cover Page**

**File name:** Lab_12_Nand_Gate_Half_Adder_circuit_Lesson
**Title:** NAND Gate Half Adder Lesson
**Subtitle:** วงจรบวกเลขฐานสองขนาดครึ่งบิตด้วย NAND Gate
**IC Label:** 7400

**Objectives:**
- เข้าใจหลักการสร้างวงจรบวกเลขฐานสองขนาดครึ่งบิต (Half Adder) ด้วย NAND Gate
- สามารถประยุกต์ใช้คุณสมบัติ Universal Gate ของ NAND Gate ในการสร้างวงจรคณิตศาสตร์
- ตรวจสอบความถูกต้องของเอาต์พุตผลบวก (SUM) และตัวนำออก (Carry-Out)

#### 12.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** วงจร Half Adder สามารถสร้างขึ้นจาก NAND Gate เพียงชนิดเดียวจำนวน 5 ตัวได้ดังนี้:
- **SUM ($S$):** สร้างฟังก์ชัน XOR จาก NAND Gate 4 ตัว $S = A \oplus B = \overline{\overline{A \cdot \overline{A \cdot B}} \cdot \overline{B \cdot \overline{A \cdot B}}}$
- **Carry Out ($C_{OUT}$):** นำสัญญาณ $\overline{A \cdot B}$ จากเอาต์พุตของ NAND ตัวแรกมากลับสัญญาณด้วย NOT Gate (NAND รวบขา) จะได้ $C_{OUT} = A \cdot B$

#### 12.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ NAND Gate ทั้งหมด 5 ตัว (IC 7400 จำนวน 2 ตัว) ในการต่อเป็นวงจร Half Adder
**Inputs:** A, B
**Outputs:** SUM, C_OUT
**Gate Type:** NAND

**Body (optional):** สัญญาณอินพุต A และ B ป้อนเข้า NAND ตัวที่ 1 ได้สัญญาณ $\overline{A \cdot B}$ แล้วส่งไปยัง NAND ตัวที่ 2, 3 และ 5 เพื่อสร้างฟังก์ชัน XOR สำหรับเอาต์พุต SUM และฟังก์ชัน AND สำหรับเอาต์พุต C_OUT ตามลำดับ

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_12_Nand_Gate_Half_Adder_circuit.drawio.svg)

#### 12.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7400
**Instructions:**
- ต่อ NAND Gate 5 ตัวบน IC 7400 ตามไดอะแกรม
- ป้อนสภาวะอินพุต A, B ทุกรูปแบบ (0+0, 0+1, 1+0, 1+1)
- ตรวจสอบเอาต์พุต SUM และ C_OUT ว่าตรงตามตารางความจริงหรือไม่

**Verification Text:** ตรวจสอบผลบวกเลขฐานสองของวงจร NAND Gate Half Adder ครบทั้ง 4 สภาวะ

**Truth Table:**
- A=0, B=0 --> SUM=0, C_OUT=0
- A=0, B=1 --> SUM=1, C_OUT=0
- A=1, B=0 --> SUM=1, C_OUT=0
- A=1, B=1 --> SUM=0, C_OUT=1

#### 12.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนพิสูจน์ได้ว่าสามารถใช้วงจร NAND Gate เพียงชนิดเดียวในการสร้างวงจร Half Adder สำหรับคำนวณ SUM และ Carry-Out ได้อย่างถูกต้อง