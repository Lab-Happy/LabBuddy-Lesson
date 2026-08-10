
### **Lab 02: 2-Input AND & OR Gates** — การเปรียบเทียบตรรกะ AND และ OR

#### 2.1 **Cover Page**
**File name:** Lab_02_AND_OR_gate_E2E_Test
**Title:** AND & OR Gate Lesson
**Subtitle:** การทดลอง AND Gate และ OR Gate
**IC Label:** 7408 / 7432

**Objectives:**
- เข้าใจหลักการทำงานของ AND Gate และ OR Gate
- สามารถสร้างวงจรเปรียบเทียบผลลัพธ์ตรรกะแบบคูณ (AND) และแบบบวก (OR)
- สามารถทดสอบผลลัพธ์ด้วยตารางความจริง 2 อินพุต

#### 2.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** AND Gate ทำหน้าที่บูลีนคูณ ($Y = A \cdot B$) ผลลัพธ์จะเป็น 1 เมื่ออินพุตทั้งสองเป็น 1 เท่านั้น ส่วน OR Gate ทำหน้าที่บูลีนบวก ($Y = A + B$) ผลลัพธ์จะเป็น 1 เมื่อมีอินพุตใดอินพุตหนึ่งเป็น 1

#### 2.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ต่อสายบน protoboard โดยใช้ IC 7408 (AND) และ IC 7432 (OR)
**Inputs:** A, B
**Outputs:** Y_AND, Y_OR
**Gate Type:** AND, OR

**Body (optional):** ป้อนสัญญาณอินพุต A และ B ร่วมกันไปยังทั้ง AND Gate และ OR Gate แล้วสังเกตความแตกต่างของเอาต์พุต Y_AND และ Y_OR ผ่านหลอดแสดงผล LED


![](100-Projects/103-LabBuddy/08_Labsheet/Lab_02_And_Or/Lab_02_And_Or_circuit.drawio.svg)


#### 2.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7408 / 7432
**Instructions:**
- ต่อวงจรอินพุต A, B เข้ากับขาเกต
- ป้อนสภาวะอินพุตทั้ง 4 แบบ แล้วกดปุ่มตรวจสอบ

**Verification Text:** ตรวจสอบสภาวะอินพุตทั้ง 4 สภาวะตามตารางความจริงเพื่อยืนยันการทำงานของ AND และ OR Gate

**Truth Table:**
- A=0, B=0 --> Y_AND=0, Y_OR=0
- A=0, B=1 --> Y_AND=0, Y_OR=1
- A=1, B=0 --> Y_AND=0, Y_OR=1
- A=1, B=1 --> Y_AND=1, Y_OR=1

#### 2.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนสามารถเข้าใจข้อแตกต่างระหว่าง AND Gate และ OR Gate ได้อย่างถูกต้อง