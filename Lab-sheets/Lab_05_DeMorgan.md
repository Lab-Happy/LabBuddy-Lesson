
### **Lab 05: De Morgan's Laws (กฎของเดอมอร์แกน)** — พิสูจน์สมการ $\overline{A \cdot B} = \overline{A} + \overline{B}$

#### 5.1 **Cover Page**
**File name:** Lab_05_DeMorgan_circuit_Lesson
**Title:** De Morgan's Laws Lesson
**Subtitle:** การพิสูจน์กฎของเดอมอร์แกน
**IC Label:** 7400 / 7404 / 7432

**Objectives:**
- เข้าใจทฤษฎีกฎของเดอมอร์แกนในพีชคณิตบูลีน
- พิสูจน์ว่า $\overline{A \cdot B}$ มีค่าเท่ากับ $\overline{A} + \overline{B}$
- สามารถประกอบวงจรเปรียบเทียบทั้งสองฝั่งของสมการ

#### 5.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** กฎของเดอมอร์แกนระบุว่า:
1. $\overline{A \cdot B} = \overline{A} + \overline{B}$ (NAND เท่ากับ Negative-OR)
2. $\overline{A + B} = \overline{A} \cdot \overline{B}$ (NOR เท่ากับ Negative-AND)

#### 5.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบวงจร 2 ด้าน: ฝั่งซ้ายใช้ NAND Gate และฝั่งขวาใช้ NOT 2 ตัวต่อเข้า OR Gate
**Inputs:** A, B
**Outputs:** Y_LHS, Y_RHS
**Gate Type:** NAND, NOT, OR

**Body (optional):** ป้อนอินพุต A, B เดียวกันให้ทั้ง 2 วงจร สังเกตว่าเอาต์พุต Y_LHS และ Y_RHS มีค่าเท่ากันทุกกรณีสภาวะ


![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_05_De_Morgan_circuit.drawio.svg)

#### 5.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7400, 7404, 7432
**Instructions:**
- ต่อวงจรตามไดอะแกรมทั้งสองฝั่ง
- ตรวจสอบว่าเอาต์พุต Y_LHS และ Y_RHS ตรงกันทุกสภาวะ

**Verification Text:** ทดสอบสภาวะอินพุตทั้ง 4 แบบเพื่อยืนยันความเท่ากันของสมการตามกฎของเดอมอร์แกน

**Truth Table:**
- A=0, B=0 --> Y_LHS=1, Y_RHS=1
- A=0, B=1 --> Y_LHS=1, Y_RHS=1
- A=1, B=0 --> Y_LHS=1, Y_RHS=1
- A=1, B=1 --> Y_LHS=0, Y_RHS=0

#### 5.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนสามารถพิสูจน์กฎของเดอมอร์แกนด้วยฮาร์ดแวร์จริงและเข้าใจการลดรูปสมการบูลีนได้อย่างสมบูรณ์