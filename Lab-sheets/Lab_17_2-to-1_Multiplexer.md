### **Lab 17: 2-to-1 Multiplexer (MUX)** — วงจรเลือกสลับสัญญาณข้อมูลด้วย Select Line ($S$)

#### 17.1 **Cover Page**
**File name:** Lab_17_2-to-1_Multiplexer_circuit_Lesson
**Title:** 2-to-1 Multiplexer Lesson
**Subtitle:** วงจรเลือกสลับสัญญาณข้อมูลดิจิทัลขนาด 2-to-1
**IC Label:** 74157 / 7404 / 7408 / 7432

**Objectives:**
- เข้าใจหลักการทำงานของ Multiplexer (Data Selector)
- สร้างวงจร 2-to-1 MUX เลือกช่องสัญญาณข้อมูลด้วยสาย Select ($S$)
- เรียนรู้การสวิตช์ข้อมูลหลายช่องลงบนสายส่งสัญญาณเส้นเดียว

#### 17.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Multiplexer ทำหน้าที่เลือกสัญญาณข้อมูลจากหลายช่องอินพุต ($I_0, I_1$) ออกไปยังเอาต์พุต $Y$ เพียงช่องเดียว โดยมีสาย Select ($S$) เป็นตัวควบคุม:
- เมื่อ $S = 0 \rightarrow Y = I_0$
- เมื่อ $S = 1 \rightarrow Y = I_1$
สมการบูลีน: $Y = \overline{S} \cdot I_0 + S \cdot I_1$

#### 17.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบด้วย NOT Gate 1 ตัว, AND Gate 2 ตัว และ OR Gate 1 ตัว
**Inputs:** I0, I1, S
**Outputs:** Y
**Gate Type:** NOT, AND, OR

**Body (optional):** สาย Select (S) ต่อตรงเข้า AND ตัวที่ 2 และต่อผ่าน NOT เข้า AND ตัวที่ 1 เพื่อเลือกผ่านสัญญาณ I0 หรือ I1

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_17_2-to-1_Multiplexer_circuit.drawio.svg)

#### 17.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 74157 / 7404, 7408, 7432
**Instructions:**
- ทดสอบสลับสัญญาณ Select S=0 แล้วเปลี่ยนค่า I0 เพื่อดูว่า Y เปลี่ยนตาม I0 หรือไม่
- ทดสอบสลับสัญญาณ Select S=1 แล้วเปลี่ยนค่า I1 เพื่อดูว่า Y เปลี่ยนตาม I1 หรือไม่

**Verification Text:** ตรวจสอบว่าเอาต์พุต Y เลือกส่งผ่านข้อมูลจาก I0 หรือ I1 ตามสภาวะสาย Select S

**Truth Table:**
- S=0, I0=0, I1=0 --> Y=0
- S=0, I0=0, I1=1 --> Y=0
- S=0, I0=1, I1=0 --> Y=1
- S=0, I0=1, I1=1 --> Y=1
- S=1, I0=0, I1=0 --> Y=0
- S=1, I0=0, I1=1 --> Y=1
- S=1, I0=1, I1=0 --> Y=0
- S=1, I0=1, I1=1 --> Y=1

#### 17.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจการทำงานของ Multiplexer ในการเลือกสลับช่องสัญญาณข้อมูลดิจิทัลได้อย่างถูกต้อง
