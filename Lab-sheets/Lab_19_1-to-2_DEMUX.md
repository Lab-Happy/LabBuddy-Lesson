### **Lab 19: 1-to-2 Demultiplexer (DEMUX)** — วงจรกระจายสัญญาณข้อมูลดิจิทัล

#### 19.1 **Cover Page**
**File name:** Lab_19_1-to-2_DEMUX_circuit_Lesson
**Title:** 1-to-2 Demultiplexer Lesson
**Subtitle:** วงจรกระจายสัญญาณข้อมูลดิจิทัล 1-to-2
**IC Label:** 74139 / 7404 / 7408

**Objectives:**
- เข้าใจหลักการทำงานของ Demultiplexer (Data Distributor)
- สามารถกระจายสัญญาณข้อมูลอินพุต ($D$) ออกไปยังเอาต์พุต 2 ช่อง ($Y_0, Y_1$) ด้วยสาย Select ($S$)
- เรียนรู้การสวิตช์ข้อมูลจากสายส่งเดียวไปยังหลายปลายทาง

#### 19.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Demultiplexer ทำหน้าที่ตรงข้ามกับ Multiplexer โดยรับสัญญาณข้อมูลอินพุต $D$ เพียงช่องเดียว แล้วเลือกส่งออกไปยังเอาต์พุตช่องใดช่องหนึ่ง ($Y_0, Y_1$) ขึ้นอยู่กับสายควบคุม Select ($S$):
- เมื่อ $S = 0 \rightarrow Y_0 = D, Y_1 = 0$
- เมื่อ $S = 1 \rightarrow Y_0 = 0, Y_1 = D$
สมการบูลีน: $Y_0 = \overline{S} \cdot D$, $Y_1 = S \cdot D$

#### 19.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบด้วย NOT Gate 1 ตัว และ AND Gate 2 ตัว
**Inputs:** D, S
**Outputs:** Y0, Y1
**Gate Type:** NOT, AND

**Body (optional):** สัญญาณข้อมูล D ป้อนเข้า AND Gate ทั้งสองตัว โดยสาย Select S ต่อตรงเข้า AND ตัวที่ 2 และผ่าน NOT Gate เข้า AND ตัวที่ 1 เพื่อเลือกส่งสัญญาณข้อมูล D ออกทาง Y0 หรือ Y1

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_19_1-to-2_DEMUX_circuit.drawio.svg)

#### 19.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 74139 / 7404, 7408
**Instructions:**
- ป้อนสภาวะสาย Select S=0 แล้วสลับสัญญาณข้อมูล D (0/1) เพื่อดูว่า Y0 เปลี่ยนตาม D หรือไม่
- ป้อนสภาวะสาย Select S=1 แล้วสลับสัญญาณข้อมูล D (0/1) เพื่อดูว่า Y1 เปลี่ยนตาม D หรือไม่

**Verification Text:** ตรวจสอบว่าเอาต์พุต Y0 หรือ Y1 ส่งผ่านข้อมูล D ตามสภาวะสาย Select S อย่างถูกต้อง

**Truth Table:**
- S=0, D=0 --> Y0=0, Y1=0
- S=0, D=1 --> Y0=1, Y1=0
- S=1, D=0 --> Y0=0, Y1=0
- S=1, D=1 --> Y0=0, Y1=1

#### 19.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจหลักการกระจายสัญญาณข้อมูลดิจิทัลด้วย 1-to-2 Demultiplexer เรียบร้อยแล้ว