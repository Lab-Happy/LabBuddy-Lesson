### **Lab 18: 4-to-1 Multiplexer (MUX)** — วงจรเลือกสลับสัญญาณข้อมูล 4 ช่องด้วย 2 Select Lines ($S_1, S_0$)

#### 18.1 **Cover Page**
**File name:** Lab_18_4-to-1_Multiplexer_circuit_Lesson
**Title:** 4-to-1 Multiplexer Lesson
**Subtitle:** วงจรเลือกสลับสัญญาณข้อมูลดิจิทัลขนาด 4-to-1
**IC Label:** 74153 / 74151

**Objectives:**
- เข้าใจหลักการทำงานของ 4-to-1 Multiplexer (Data Selector)
- สามารถเลือกส่งผ่านข้อมูล 4 ช่อง ($I_0, I_1, I_2, I_3$) ออกไปยังเอาต์พุต $Y$ เดียว ด้วยสาย Select 2 บิต ($S_1, S_0$)
- เรียนรู้การสวิตช์และรวมช่องสัญญาณข้อมูลดิจิทัลหลายสายในระบบสื่อสาร

#### 18.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** 4-to-1 Multiplexer ทำหน้าที่เลือกสัญญาณข้อมูลจากอินพุต 4 ช่อง ($I_0, I_1, I_2, I_3$) ออกไปยังเอาต์พุต $Y$ ช่องเดียว โดยใช้สาย Select 2 ช่อง ($S_1, S_0$) ในการกำหนดช่องข้อมูล:
- เมื่อ $S_1S_0 = 00 \rightarrow Y = I_0$
- เมื่อ $S_1S_0 = 01 \rightarrow Y = I_1$
- เมื่อ $S_1S_0 = 10 \rightarrow Y = I_2$
- เมื่อ $S_1S_0 = 11 \rightarrow Y = I_3$
สมการบูลีน: $Y = \overline{S_1}\cdot\overline{S_0}\cdot I_0 + \overline{S_1}\cdot S_0\cdot I_1 + S_1\cdot\overline{S_0}\cdot I_2 + S_1\cdot S_0\cdot I_3$

#### 18.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ IC 74153 (Dual 4-to-1 MUX) หรือต่อด้วย NOT 2 ตัว, AND 4 ตัว (3-input) และ OR 1 ตัว (4-input)
**Inputs:** I0, I1, I2, I3, S0, S1
**Outputs:** Y
**Gate Type:** NOT, AND, OR (หรือ IC 74153)

**Body (optional):** สาย Select $S_1, S_0$ ถูกถอดรหัสผ่าน NOT Gate เพื่อกำหนดเงื่อนไขในการส่งผ่านสัญญาณจากอินพุต $I_0, I_1, I_2, I_3$ เข้า AND Gate แต่ละตัว แล้วนำเอาต์พุตรวมเข้า OR Gate เพื่อได้สัญญาณเอาต์พุต Y

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_18_4-to-1_Multiplexer_circuit.drawio.svg)
#### 18.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 74153 / 74151
**Instructions:**
- ป้อนสภาวะสาย Select $S_1S_0 = 00, 01, 10, 11$
- ทดสอบเปลี่ยนค่าสัญญาณอินพุต $I_0, I_1, I_2, I_3$ เพื่อยืนยันว่าเอาต์พุต Y เปลี่ยนตามช่องข้อมูลที่เลือก

**Verification Text:** ตรวจสอบว่าเอาต์พุต Y เลือกส่งผ่านข้อมูลจาก $I_0, I_1, I_2, I_3$ ตามสภาวะสาย Select $S_1, S_0$ ทั้ง 4 สภาวะอย่างถูกต้อง

**Truth Table:**
- S1=0, S0=0 --> Y=D0
- S1=0, S0=1 --> Y=D1
- S1=1, S0=0 --> Y=D2
- S1=1, S0=1 --> Y=D3

#### 18.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจการทำงานของ 4-to-1 Multiplexer ในการเลือกสลับช่องสัญญาณข้อมูลดิจิทัลได้อย่างถูกต้อง
