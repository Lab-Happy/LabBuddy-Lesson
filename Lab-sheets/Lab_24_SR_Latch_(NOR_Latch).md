### **Lab 24: SR Latch (NOR Latch)** — วงจรแลตช์จำสภาวะด้วย NOR Gate (Active-High $SR$)

#### 24.1 **Cover Page**
**File name:** Lab_24_SR_Latch_NOR_Latch_circuit_Lesson
**Title:** SR Latch (NOR Latch) Lesson
**Subtitle:** วงจรแลตช์จำสภาวะ SR ด้วย NOR Gate (Active-High)
**IC Label:** 7402

**Objectives:**
- เข้าใจหลักการทำงานของ NOR SR Latch ($SR$ Latch)
- เรียนรู้สภาวะการควบคุมแบบ Active-High ($S=1 \rightarrow Set$, $R=1 \rightarrow Reset$)
- ระบุและหลีกเลี่ยงสภาวะห้ามใช้งาน (Forbidden / Invalid State $S=1, R=1$)

#### 24.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** NOR SR Latch เป็นวงจรจำสภาวะ 1 บิตแบบ Active-High ที่ใช้สัญญาณป้อนกลับ (Feedback) จาก NOR Gate 2 ตัว:
- $S=1, R=0 \rightarrow Q=1, \bar{Q}=0$ (Set)
- $S=0, R=1 \rightarrow Q=0, \bar{Q}=1$ (Reset)
- $S=0, R=0 \rightarrow$ คงค่าเดิม (Hold)
- $S=1, R=1 \rightarrow$ สภาวะห้ามใช้งาน (Forbidden / Invalid State ทำให้เอาต์พุตทั้งคู่เป็น 0)

#### 24.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ NOR Gate 2 ตัว (IC 7402) ต่อเอาต์พุตไขว้เข้าอินพุตป้อนกลับของอีกฝั่ง
**Inputs:** S, R
**Outputs:** Q, Q_N
**Gate Type:** NOR

**Body (optional):** ต่อเอาต์พุต Q ของ NOR ตัวที่ 2 ป้อนกลับเข้าเป็นอินพุตของ NOR ตัวที่ 1 (ที่มีอินพุต R) และต่อเอาต์พุต Q_N ของ NOR ตัวที่ 1 ป้อนกลับเข้าอินพุตของ NOR ตัวที่ 2 (ที่มีอินพุต S)

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_24_SR_NOR_Latch_circuit.drawio.svg)

#### 24.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7402
**Instructions:**
- ป้อนสภาวะ Active-High ($S=1, R=0$) เพื่อ Set เอาต์พุต $Q=1$
- ป้อนสภาวะ Active-High ($S=0, R=1$) เพื่อ Reset เอาต์พุต $Q=0$
- ป้อนสภาวะ Hold ($S=0, R=0$) ยืนยันว่าเอาต์พุตคงค่าเดิมไว้

**Verification Text:** ตรวจสอบวงจร NOR SR Latch ในการจำและคงสภาวะเอาต์พุต Q และ Q_N

**Truth Table:**
- S=1, R=0 --> Q=1, Q_N=0
- S=0, R=0 --> Q=1, Q_N=0
- S=0, R=1 --> Q=0, Q_N=1
- S=0, R=0 --> Q=0, Q_N=1

#### 24.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจหลักการทำงานของ NOR SR Latch (Active-High) ในการบันทึกและคงสภาวะข้อมูลดิจิทัลเรียบร้อยแล้ว