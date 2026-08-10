### **Lab 23: SR Latch (NAND Latch)** — วงจรแลตช์จำสภาวะด้วย NAND Gate (Active-Low $\bar{S}\bar{R}$)

#### 23.1 **Cover Page**
**File name:** Lab_23_SR_Latch_NAND_ Latch_circuit_Lesson
**Title:** SR Latch (NAND Latch) Lesson
**Subtitle:** วงจรแลตช์จำสภาวะ SR ด้วย NAND Gate (Active-Low)
**IC Label:** 7400

**Objectives:**
- เข้าใจหลักการทำงานของ NAND SR Latch ($\bar{S}\bar{R}$ Latch)
- เรียนรู้สภาวะการควบคุมแบบ Active-Low ($\bar{S}=0 \rightarrow Set$, $\bar{R}=0 \rightarrow Reset$)
- ระบุและหลีกเลี่ยงสภาวะห้ามใช้งาน (Forbidden / Invalid State $\bar{S}=0, \bar{R}=0$)

#### 23.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** NAND SR Latch เป็นวงจรจำสภาวะ 1 บิตแบบ Active-Low ที่ใช้สัญญาณป้อนกลับ (Feedback) จาก NAND Gate 2 ตัว:
- $\bar{S}=0, \bar{R}=1 \rightarrow Q=1, \bar{Q}=0$ (Set)
- $\bar{S}=1, \bar{R}=0 \rightarrow Q=0, \bar{Q}=1$ (Reset)
- $\bar{S}=1, \bar{R}=1 \rightarrow$ คงค่าเดิม (Hold)
- $\bar{S}=0, \bar{R}=0 \rightarrow$ สภาวะห้ามใช้งาน (Forbidden / Invalid State ทำให้เอาต์พุตทั้งคู่เป็น 1)

#### 23.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ NAND Gate 2 ตัว (IC 7400) ต่อเอาต์พุตไขว้เข้าอินพุตป้อนกลับของอีกฝั่ง
**Inputs:** S_N, R_N
**Outputs:** Q, Q_N
**Gate Type:** NAND

**Body (optional):** ต่อเอาต์พุต Q ของ NAND ตัวที่ 1 ป้อนกลับเข้าเป็นอินพุตของ NAND ตัวที่ 2 และนำเอาต์พุต Q_N ของ NAND ตัวที่ 2 ป้อนกลับเข้าเป็นอินพุตของ NAND ตัวที่ 1

![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_23_SR_Latch_circuit.drawio.svg)


#### 23.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7400
**Instructions:**
- ป้อนสภาวะ Active-Low ($\bar{S}=0, \bar{R}=1$) เพื่อ Set เอาต์พุต $Q=1$
- ป้อนสภาวะ Active-Low ($\bar{S}=1, \bar{R}=0$) เพื่อ Reset เอาต์พุต $Q=0$
- ป้อนสภาวะ Hold ($\bar{S}=1, \bar{R}=1$) ยืนยันว่าเอาต์พุตคงค่าเดิมไว้

**Verification Text:** ตรวจสอบวงจร NAND SR Latch ในการจำและคงสภาวะเอาต์พุต Q และ Q_N

**Truth Table:**
- S_N=0, R_N=1 --> Q=1, Q_N=0
- S_N=1, R_N=1 --> Q=1, Q_N=0
- S_N=1, R_N=0 --> Q=0, Q_N=1
- S_N=1, R_N=1 --> Q=0, Q_N=1

#### 23.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจหลักการทำงานของ NAND SR Latch (Active-Low) ในการบันทึกและคงสภาวะข้อมูลดิจิทัลเรียบร้อยแล้ว