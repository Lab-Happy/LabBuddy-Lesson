### **Lab 25: Gated D Latch** — วงจรแลตช์บันทึกข้อมูลพร้อมสัญญาณควบคุม (Enable)

#### 25.1 **Cover Page**
**File name:** Lab_25_Gated_D_Latch_circuit_Lesson
**Title:** Gated D Latch Lesson
**Subtitle:** วงจรแลตช์บันทึกข้อมูลชนิด D พร้อมสัญญาณ Enable
**IC Label:** 7475 / 7400 / 7404

**Objectives:**
- เข้าใจหลักการทำงานของ Gated D Latch (Data Latch)
- ป้องกันสภาวะห้ามใช้งาน (Invalid State) ของ SR Latch โดยการใช้สัญญาณ $D$ และ Inverter
- เรียนรู้บทบาทของสัญญาณ Enable ($E$) ในการควบคุมจังหวะบันทึกข้อมูล (Transparent & Hold Mode)

#### 25.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** Gated D Latch แก้ไขข้อผิดพลาดของ SR Latch โดยใช้อินพุต $D$ เพียงช่องเดียว และใช้สัญญาณ Enable ($E$) ควบคุมจังหวะการบันทึก:
- เมื่อ $E = 1 \rightarrow Q = D$ (Transparent Mode เอาต์พุตเปลี่ยนตามอินพุต D)
- เมื่อ $E = 0 \rightarrow Q$ คงค่าเดิมก่อนหน้า (Latch / Hold Mode สัญญาณ D ไม่มีผลต่อเอาต์พุต)

#### 25.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบด้วย NOT Gate 1 ตัว (ต่อระหว่าง D ไปยัง R) และ NAND Gate 4 ตัว
**Inputs:** D, E
**Outputs:** Q, Q_N
**Gate Type:** NOT, NAND (หรือ IC 7475)

**Body (optional):** สัญญาณ D และสัญญาณตรงข้าม ($\overline{D}$) ถูกควบคุมผ่าน NAND Gate ด้วยสัญญาณ Enable E ก่อนป้อนเข้าสู่ NAND SR Latch เพื่อส่งผ่านหรือบันทึกข้อมูล

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_25_Gated_D_Latch_circuit.svg)

#### 25.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7475 / 7400, 7404
**Instructions:**
- ป้อน E=1 แล้วเปลี่ยนสภาวะ D (0/1) เพื่อดูว่า Q เปลี่ยนตาม D หรือไม่ (Transparent Mode)
- ป้อน E=0 แล้วเปลี่ยนสภาวะ D เพื่อยืนยันว่า Q ไม่เปลี่ยนแปลง (Hold Mode)

**Verification Text:** ตรวจสอบวงจร Gated D Latch ในการส่งผ่านข้อมูลเมื่อ E=1 และจำค่าเดิมเมื่อ E=0

**Truth Table:**
- E=1, D=0 --> Q=0, Q_N=1
- E=1, D=1 --> Q=1, Q_N=0
- E=0, D=0 --> Q=1, Q_N=0
- E=0, D=1 --> Q=1, Q_N=0

#### 25.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจการควบคุมการบันทึกข้อมูลด้วย Gated D Latch เรียบร้อยแล้ว