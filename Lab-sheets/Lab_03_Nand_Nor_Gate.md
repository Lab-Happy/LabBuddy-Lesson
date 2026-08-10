
### **Lab 03: NAND & NOR Gates (Universal Gates)** — เกตตรรกะตรงข้ามและการจัดวาง Inverter Bubble (DOT)

https://www.geeksforgeeks.org/digital-logic/what-is-nand-gate/

https://www.geeksforgeeks.org/digital-logic/nor-gate/

https://www.geeksforgeeks.org/digital-logic/or-gate/


#### 3.1 **Cover Page**
**File name:** Lab_03_Nand_Nor_Gate_circuit_Lesson
**Title:** NAND & NOR Gate Lesson
**Subtitle:** การทดลอง NAND Gate และ NOR Gate
**IC Label:** 7400 / 7402

**Objectives:**
- เข้าใจหลักการทำงานของ NAND Gate และ NOR Gate
- สังเกตผลของ Inverter Bubble (DOT) ที่ต่อท้ายเกตพื้นฐาน
- สามารถทดสอบผลลัพธ์ตรรกะตรงข้ามด้วยตารางความจริง

#### 3.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** NAND Gate คือ AND Gate ที่ต่อกลับค่าเอาต์พุตด้วย NOT ($Y = \overline{A \cdot B}$) ส่วน NOR Gate คือ OR Gate ที่ต่อกลับค่าเอาต์พุตด้วย NOT ($Y = \overline{A + B}$) ทั้งสองเกตถูกเรียกว่า Universal Gate เพราะสามารถนำมาประกอบเป็นเกตตรรกะอื่นได้ทุกประเภท

#### 3.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ต่อสายบน protoboard โดยใช้ IC 7400 (NAND) และ IC 7402 (NOR)
**Inputs:** A, B
**Outputs:** Y_NAND, Y_NOR
**Gate Type:** NAND, NOR

**Body (optional):** ต่อสวิตช์อินพุต A และ B เข้าขาเกตสังเกตการตำแหน่ง Bubble วงกลมที่ปลายเอาต์พุตของ NAND และ NOR Gate


![](100-Projects/103-LabBuddy/08_Labsheet/Lab_03_Nand_Nor_Gate/Lab_03_Nand_Nor_Gate_circuit.drawio.svg)


#### 3.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7400 / 7402
**Instructions:**
- ต่อวงจรเข้ากับไอซี 7400 และ 7402
- ป้อนสภาวะอินพุตทั้ง 4 แบบเพื่อตรวจสอบเอาต์พุต

**Verification Text:** ตรวจสอบผลลัพธ์ของ NAND และ NOR Gate ว่าเป็นค่าตรงข้ามกับ AND และ OR Gate หรือไม่

**Truth Table:**
- A=0, B=0 --> Y_NAND=1, Y_NOR=1
- A=0, B=1 --> Y_NAND=1, Y_NOR=0
- A=1, B=0 --> Y_NAND=1, Y_NOR=0
- A=1, B=1 --> Y_NAND=0, Y_NOR=0

#### 3.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจการทำงานของ NAND และ NOR Gate ซึ่งให้ผลลัพธ์ตรงข้ามกับ AND และ OR Gate อย่างสมบูรณ์