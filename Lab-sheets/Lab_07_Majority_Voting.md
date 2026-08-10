
### **Lab 07: Majority Voting Circuit (วงจรโหวตเสียงข้างมาก)** — วงจรการตัดสินใจ 3 อินพุต ($A, B, C$)

#### 7.1 **Cover Page**
**File name:** Lab_07_Majority_Voting_circuit_Lesson
**Title:** Majority Voting Circuit Lesson
**Subtitle:** วงจรตัดสินใจเสียงข้างมาก 3 อินพุต
**IC Label:** 7408 / 7432

**Objectives:**
- เข้าใจการออกแบบวงจรตัดสินใจตามเงื่อนไขทางลอจิก
- สร้างวงจร Majority Logic $Y = A \cdot B + B \cdot C + A \cdot C$
- ทดสอบวงจรที่มีอินพุต 3 ชาแนล ($A, B, C$)

#### 7.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** วงจร Majority Voter เป็นวงจรตัดสินใจที่จะให้เอาต์พุตเป็น 1 เมื่อมีสัญญาณอินพุตอย่างน้อย 2 ใน 3 อินพุตเป็น 1 มีสมการเป็น $Y = A \cdot B + B \cdot C + A \cdot C$

#### 7.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ต่อ AND Gate 3 ตัวสำหรับจับคู่ $AB, BC, AC$ แล้วนำเอาต์พุตทั้ง 3 เข้า OR Gate แบบ 3 อินพุต
**Inputs:** A, B, C
**Outputs:** Y
**Gate Type:** AND, OR

**Body (optional):** ต่อสายสัญญาณอินพุต A, B, C กระจายไปยัง AND Gate 3 ชุด และใช้จุด Junction เชื่อมต่อสัญญาณร่วมกัน


![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_07_Majority_Voting_Circuit.drawio.svg)


#### 7.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7408, 7432
**Instructions:**
- ทดสอบป้อนสัญญาณอินพุตทั้ง 8 สภาวะ ($2^3 = 8$)
- ยืนยันว่าเอาต์พุต Y เป็น 1 เมื่อมีอินพุตเป็น 1 ตั้งแต่ 2 ขาขึ้นไป

**Verification Text:** ตรวจสอบการทำงานของวงจร Majority Voter ครบทั้ง 8 สภาวะตรรกะ

**Truth Table:**
- A=0, B=0, C=0 --> Y=0
- A=0, B=0, C=1 --> Y=0
- A=0, B=1, C=0 --> Y=0
- A=0, B=1, C=1 --> Y=1
- A=1, B=0, C=0 --> Y=0
- A=1, B=0, C=1 --> Y=1
- A=1, B=1, C=0 --> Y=1
- A=1, B=1, C=1 --> Y=1

#### 7.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจการประยุกต์ใช้วงจรตรรกะผสม 3 อินพุตในการสร้างระบบตัดสินใจเสียงข้างมากได้อย่างถูกต้อง