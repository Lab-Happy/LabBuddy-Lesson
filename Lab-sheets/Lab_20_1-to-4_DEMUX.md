### **Lab 20: 1-to-4 Demultiplexer (DEMUX)** — วงจรกระจายสัญญาณข้อมูลดิจิทัล 4 ช่อง

#### 20.1 **Cover Page**
**File name:** Lab_20_1-to-4_DEMUX_circuit_Lesson
**Title:** 1-to-4 Demultiplexer Lesson
**Subtitle:** วงจรกระจายสัญญาณข้อมูลดิจิทัล 1-to-4
**IC Label:** 74139 / 74155

**Objectives:**
- เข้าใจหลักการทำงานของ 1-to-4 Demultiplexer
- สามารถเลือกกระจายสัญญาณข้อมูลอินพุต ($D$) ออกไปยังเอาต์พุต 4 ช่อง ($Y_0, Y_1, Y_2, Y_3$) ด้วยสาย Select 2 บิต ($S_1, S_0$)
- เรียนรู้การสวิตช์สายสัญญาณข้อมูลไปยังปลายทางหลายจุด

#### 20.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** 1-to-4 Demultiplexer รับสัญญาณข้อมูลอินพุต $D$ เพียงช่องเดียว แล้วถอดรหัสสาย Select 2 ช่อง ($S_1, S_0$) เพื่อเลือกส่งออกไปยังเอาต์พุตเพียงช่องเดียว ($Y_0, Y_1, Y_2, Y_3$):
- $S_1S_0 = 00 \rightarrow Y_0 = D$
- $S_1S_0 = 01 \rightarrow Y_1 = D$
- $S_1S_0 = 10 \rightarrow Y_2 = D$
- $S_1S_0 = 11 \rightarrow Y_3 = D$
สมการบูลีน:
$Y_0 = \overline{S_1} \cdot \overline{S_0} \cdot D$, $Y_1 = \overline{S_1} \cdot S_0 \cdot D$, $Y_2 = S_1 \cdot \overline{S_0} \cdot D$, $Y_3 = S_1 \cdot S_0 \cdot D$

#### 20.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบด้วย NOT Gate 2 ตัว (สำหรับ $S_1, S_0$) และ AND Gate 4 ตัว (แบบ 3-input)
**Inputs:** D, S0, S1
**Outputs:** Y0, Y1, Y2, Y3
**Gate Type:** NOT, AND (หรือ IC 74139)

**Body (optional):** สัญญาณข้อมูล D ป้อนเข้า AND Gate ทั้ง 4 ตัว โดยสาย Select $S_1, S_0$ ถูกถอดรหัสผ่าน NOT Gate เพื่อเปิดสัญญาณให้ AND Gate ของเอาต์พุต $Y_0, Y_1, Y_2, Y_3$ ตามลำดับ

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_20_1-to-4_DEMUX_circuit.drawio.svg)

#### 20.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 74139 / 74155
**Instructions:**
- ป้อนสภาวะสาย Select $S_1S_0 = 00, 01, 10, 11$
- ทดสอบเปลี่ยนสภาวะข้อมูล D (0/1) เพื่อดูว่าเอาต์พุตช่องที่เลือกเปลี่ยนตาม D และช่องอื่นเป็น 0

**Verification Text:** ตรวจสอบวงจร 1-to-4 Demultiplexer กระจายสัญญาณข้อมูล D ออกเอาต์พุต $Y_0, Y_1, Y_2, Y_3$ ตามสาย Select $S_1, S_0$ ครบถ้วน

**Truth Table:**
- S1=0, S0=0, D=1 --> Y0=1, Y1=0, Y2=0, Y3=0
- S1=0, S0=1, D=1 --> Y0=0, Y1=1, Y2=0, Y3=0
- S1=1, S0=0, D=1 --> Y0=0, Y1=0, Y2=1, Y3=0
- S1=1, S0=1, D=1 --> Y0=0, Y1=0, Y2=0, Y3=1

#### 20.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจการทำงานของ 1-to-4 Demultiplexer ในการถอดรหัสและกระจายสัญญาณข้อมูลดิจิทัลได้อย่างถูกต้อง