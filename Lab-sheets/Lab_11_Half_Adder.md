
### **Lab 11: Half Adder (วงจรบวกเลขครึ่งบิต)** — XOR + AND ($SUM$ & $C_{OUT}$)

#### 11.1 **Cover Page**
**File name:** Lab_11_Half_Adder_circuit_Lesson
**Title:** Half Adder Lesson
**Subtitle:** วงจรบวกเลขฐานสองขนาดครึ่งบิต
**IC Label:** 7486 / 7408

**Objectives:**
- เข้าใจหลักการบวกเลขฐานสองระดับบิตพื้นฐาน
- สร้างวงจร Half Adder โดยใช้ XOR Gate และ AND Gate
- แยกเอาต์พุตผลบวก (SUM) และตัวนำออก (Carry-Out)

#### 11.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Half Adder ทำหน้าที่บวกเลขฐานสอง 1 บิตจำนวน 2 อินพุต ($A, B$) มีเอาต์พุต 2 ช่อง:
- **SUM ($S$):** ผลบวกตรรกะ $S = A \oplus B$
- **Carry Out ($C_{OUT}$):** ตัวนำออก $C_{OUT} = A \cdot B$

#### 11.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ต่อสวิตช์ A, B ขนานไปยังทั้ง XOR Gate และ AND Gate
**Inputs:** A, B
**Outputs:** SUM, C_OUT
**Gate Type:** XOR, AND

**Body (optional):** สัญญาณ A และ B จะแตกกิ่ง (Junction) เข้า XOR Gate เพื่อคำนวณค่า SUM และเข้า AND Gate เพื่อคำนวณค่า C_OUT

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_11_Half_Adder_Circuit.drawio.svg)


#### 11.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7486, 7408
**Instructions:**
- ป้อนสภาวะการบวกเลข 0+0, 0+1, 1+0, 1+1
- ตรวจสอบเอาต์พุต SUM และ C_OUT

**Verification Text:** ตรวจสอบผลบวกเลขฐานสอง Half Adder ครบทั้ง 4 สภาวะ

**Truth Table:**
- A=0, B=0 --> SUM=0, C_OUT=0
- A=0, B=1 --> SUM=1, C_OUT=0
- A=1, B=0 --> SUM=1, C_OUT=0
- A=1, B=1 --> SUM=0, C_OUT=1

#### 11.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจหลักการคำนวณบวกเลขฐานสองระดับพื้นฐานด้วย Half Adder เรียบร้อยแล้ว