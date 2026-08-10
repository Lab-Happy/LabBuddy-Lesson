
### **Lab 04: XOR & XNOR Gates** — เกตเปรียบเทียบความเหมือนและความต่าง (Parity Check)

#### 4.1 **Cover Page**
**File name:** Lab_04_Xor_Xnor_Gate_circuit_Lesson
**Title:** XOR & XNOR Gate Lesson
**Subtitle:** การทดลอง Exclusive-OR และ Exclusive-NOR Gate
**IC Label:** 7486 / 74266

**Objectives:**
- เข้าใจหลักการทำงานของ XOR Gate และ XNOR Gate
- เรียนรู้การนำ XOR มาใช้เป็นวงจรตรวจจับความต่าง และ XNOR เป็นวงจรตรวจจับความเหมือน
- สามารถทดสอบผลลัพธ์ด้วยตารางความจริง

#### 4.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** XOR (Exclusive-OR) จะให้เอาต์พุตเป็น 1 เมื่ออินพุตทั้งสองมีค่าต่างกัน ($Y = A \oplus B$) ส่วน XNOR (Exclusive-NOR) จะให้เอาต์พุตเป็น 1 เมื่ออินพุตทั้งสองมีค่าเหมือนกัน ($Y = \overline{A \oplus B}$)

#### 4.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ต่อสายบน protoboard โดยใช้ IC 7486 (XOR)
**Inputs:** A, B
**Outputs:** Y_XOR, Y_XNOR
**Gate Type:** XOR, XNOR

**Body (optional):** ต่อสวิตช์ A และ B เข้ากับ XOR Gate และ XNOR Gate สังเกตเอาต์พุตเมื่ออินพุตเหมือนกันและต่างกัน


![](100-Projects/103-LabBuddy/08_Labsheet/Lab_04_Xor_Xnor_Gate/Lab_04_Xor_Xnor_Gate_circuit.drawio.svg)

#### 4.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7486 / 74266
**Instructions:**
- ต่อวงจรอินพุต A, B เข้าขาเกต
- ตรวจสอบเอาต์พุตสภาวะความต่างและความเหมือน

**Verification Text:** ทดสอบสภาวะอินพุตทั้ง 4 แบบ ตรวจสอบว่า XOR ให้ 1 เมื่อต่างกัน และ XNOR ให้ 1 เมื่อเหมือนกัน

**Truth Table:**
- A=0, B=0 --> Y_XOR=0, Y_XNOR=1
- A=0, B=1 --> Y_XOR=1, Y_XNOR=0
- A=1, B=0 --> Y_XOR=1, Y_XNOR=0
- A=1, B=1 --> Y_XOR=0, Y_XNOR=1

#### 4.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนสามารถประยุกต์ใช้ XOR ในการตรวจสอบความต่าง และ XNOR ในการตรวจสอบความเหมือนของข้อมูลได้อย่างถูกต้อง