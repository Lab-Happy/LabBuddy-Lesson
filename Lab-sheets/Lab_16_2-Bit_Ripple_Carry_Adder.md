### **Lab 16: 2-Bit Ripple Carry Adder** — การต่ออนุกรม Full Adder 2 ชุดเข้าด้วยกัน

#### 16.1 **Cover Page**
**File name:** Lab_16_2-Bit_Ripple_Carry_Adder_circuit_Lesson
**Title:** 2-Bit Ripple Carry Adder Lesson
**Subtitle:** วงจรบวกเลขฐานสอง 2 บิตแบบส่งผ่านตัวนำ
**IC Label:** 7483 หรือ 7486 / 7408 / 7432

**Objectives:**
- เรียนรู้การขยายขนาดวงจรบวกเลขจาก 1 บิตเป็น 2 บิต ($A_1A_0 + B_1B_0$)
- เข้าใจการส่งผ่านตัวนำ (Ripple Carry) จากบิตต่ำ ($C_0$) ไปยังบิตสูง ($C_1$)
- ทดสอบผลบวก 2 บิตพร้อมตัวนำออกสุดท้าย ($C_{OUT}$)

#### 16.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Ripple Carry Adder ประกอบด้วย Full Adder ต่ออนุกรมกัน โดยตัวนำออก $C_{OUT0}$ ของบิตแรก ($A_0, B_0$) จะส่งต่อเป็นตัวนำเข้า $C_{IN1}$ ของบิตถัดไป ($A_1, B_1$)

#### 16.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบ Full Adder 2 ชุด ต่อสายตัวนำเชื่อมระหว่างบล็อกบิต 0 และบิต 1
**Inputs:** A0, A1, B0, B1
**Outputs:** S0, S1, C_OUT
**Gate Type:** Full Adder Blocks (XOR, AND, OR)

**Body (optional):** ต่ออินพุต A0, B0 เข้า Full Adder บิตที่ 0 และต่อ A1, B1 เข้า Full Adder บิตที่ 1 โดยเชื่อมสาย C_OUT0 เข้า C_IN1

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_16_2-Bit_Ripple_Carry_Adder_circuit.drawio.svg)

#### 16.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7486, 7408, 7432
**Instructions:**
- ทดสอบการบวกเลข 2 บิต เช่น $01_2 + 01_2 = 10_2$ ($1+1=2$) และ $11_2 + 01_2 = 100_2$ ($3+1=4$)
- ตรวจสอบผลบวก S0, S1 และตัวนำออก C_OUT

**Verification Text:** ตรวจสอบการส่งผ่านตัวนำ Ripple Carry ระหว่างบิต 0 และบิต 1

**Truth Table (ตัวอย่างสภาวะสำคัญ):**
- A1A0=01, B1B0=01 --> S1S0=10, C_OUT=0
- A1A0=10, B1B0=01 --> S1S0=11, C_OUT=0
- A1A0=11, B1B0=01 --> S1S0=00, C_OUT=1
- A1A0=11, B1B0=11 --> S1S0=10, C_OUT=1

#### 16.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนสามารถเชื่อมต่อวงจรบวกหลายบิตแบบ Ripple Carry และเข้าใจสถาปัตยกรรมหน่วยคำนวณ ALU เบื้องต้นได้สำเร็จ