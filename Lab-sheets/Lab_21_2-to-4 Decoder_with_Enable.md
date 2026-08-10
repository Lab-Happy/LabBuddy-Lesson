### **Lab 21: 2-to-4 Decoder with Enable** — วงจรถอดรหัสรหัสฐานสองพร้อมสัญญาณเปิดการทำงาน

#### 21.1 **Cover Page**
**File name:** Lab_21_2-to-4 Decoder_with_Enable_circuit_Lesson
**Title:** 2-to-4 Decoder with Enable Lesson
**Subtitle:** วงจรถอดรหัสรหัสฐานสอง 2-to-4 แบบมีขา Enable
**IC Label:** 74139 / 74138

**Objectives:**
- เข้าใจหลักการทำงานของ Decoder (ถอดรหัสสัญญาณรหัสเป็น Active Output)
- เรียนรู้บทบาทของขา Enable ($E$) ในการควบคุมเปิด/ปิดการทำงานของวงจร
- สามารถประยุกต์ใช้วงจรถอดรหัสในการเลือกอุปกรณ์ (Chip Select / Memory Address Decoding)

#### 21.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** 2-to-4 Decoder แปลงรหัสอินพุต 2 บิต ($A_1, A_0$) ออกเป็นเอาต์พุต 4 ช่อง ($Y_0, Y_1, Y_2, Y_3$) โดยมีขา Enable ($E$) ควบคุม:
- เมื่อ $E = 0 \rightarrow$ วงจรปิดการทำงาน เอาต์พุตทุกช่องเป็น 0
- เมื่อ $E = 1 \rightarrow$ วงจรเปิดการทำงาน ถอดรหัสเลือกเอาต์พุตช่องเดียวเป็น 1 ตามรหัส $A_1A_0$:
  - $A_1A_0 = 00 \rightarrow Y_0 = 1$
  - $A_1A_0 = 01 \rightarrow Y_1 = 1$
  - $A_1A_0 = 10 \rightarrow Y_2 = 1$
  - $A_1A_0 = 11 \rightarrow Y_3 = 1$

#### 21.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ประกอบด้วย NOT Gate 2 ตัว (สำหรับ $A_1, A_0$) และ AND Gate 4 ตัว (แบบ 3-input รวมขา E)
**Inputs:** A0, A1, E
**Outputs:** Y0, Y1, Y2, Y3
**Gate Type:** NOT, AND (หรือ IC 74139)

**Body (optional):** สัญญาณ Enable E ป้อนเข้า AND Gate ทั้ง 4 ตัวร่วมกับสัญญาณอินพุต $A_1, A_0$ ที่ผ่าน NOT Gate ถอดรหัสเพื่อเปิดเอาต์พุต $Y_0, Y_1, Y_2, Y_3$


![](100-Projects/103-LabBuddy/08_Labsheet/Images/Lab_21_2-to-4%20Decoder_circuit.drawio.svg)

#### 21.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 74139 / 74138
**Instructions:**
- ทดสอบป้อน E=0 แล้วเปลี่ยนสภาวะ $A_1A_0$ เพื่อยืนยันว่าเอาต์พุตทุกช่องเป็น 0
- ป้อน E=1 แล้วทดสอบสภาวะ $A_1A_0 = 00, 01, 10, 11$ เพื่อยืนยันเอาต์พุต $Y_0, Y_1, Y_2, Y_3$

**Verification Text:** ตรวจสอบการถอดรหัสของวงจร 2-to-4 Decoder และฟังก์ชันการคุมด้วยขา Enable E

**Truth Table:**
- E=0, A1=0, A0=0 --> Y0=0, Y1=0, Y2=0, Y3=0
- E=1, A1=0, A0=0 --> Y0=1, Y1=0, Y2=0, Y3=0
- E=1, A1=0, A0=1 --> Y0=0, Y1=1, Y2=0, Y3=0
- E=1, A1=1, A0=0 --> Y0=0, Y1=0, Y2=1, Y3=0
- E=1, A1=1, A0=1 --> Y0=0, Y1=0, Y2=0, Y3=1

#### 21.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจหลักการถอดรหัสรหัสฐานสองและการควบคุมเปิด/ปิดการทำงานด้วยขา Enable ได้สำเร็จ