### **Lab 27: 2-Bit Asynchronous Binary Counter** — วงจรนับเลขฐานสองขนาด 2 บิตแบบไม่ซิงโครนัส

#### 27.1 **Cover Page**
**File name:** Lab_27_2-Bit_Asynchronous_Binary_Counter_circuit_Lesson
**Title:** 2-Bit Asynchronous Counter Lesson
**Subtitle:** วงจรนับเลขฐานสองขนาด 2 บิตแบบไร้จังหวะร่วม (Ripple Counter)
**IC Label:** 7474 / 7476 / 7493

**Objectives:**
- เข้าใจการทำงานของวงจรนับ (Binary Counter)
- สร้างวงจรนับ 2 บิต ($Q_1Q_0$) ที่สามารถนับค่าจาก 0 ถึง 3 ($00_2 \rightarrow 01_2 \rightarrow 10_2 \rightarrow 11_2 \rightarrow 00_2$)
- เรียนรู้กลไก Ripple Counter โดยนำเอาต์พุต $\bar{Q}$ ป้อนกลับเข้า $D$ และนำเอาต์พุต $Q_0$ ไปเป็นนาฬิกาให้บิตถัดไป ($Q_1$)

#### 27.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** วงจรนับแบบ Asynchronous (Ripple Counter) ใช้ Flip-Flop ต่ออนุกรมกัน โดย Flip-Flop ตัวแรกรับสัญญาณนาฬิกา $CLK$ ภายนอก ส่วน Flip-Flop ตัวถัดไปรับสัญญาณนาฬิกาจากเอาต์พุตของ Flip-Flop บิตต่ำกว่า:
- Toggle Mode: ป้อนสัญญาณ $\bar{Q}$ กลับเข้าอินพุต $D$ ของตัวเอง เพื่อให้ Flip-Flop สลับสภาวะ (Toggle) ทุกครั้งที่เกิดขอบขาขึ้นที่ $CLK$
- การนับแบบ 2 บิต จะเกิดลำดับสภาวะ 4 สภาวะ: $00_2 (0) \rightarrow 01_2 (1) \rightarrow 10_2 (2) \rightarrow 11_2 (3) \rightarrow 00_2 (0)$

#### 27.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ D Flip-Flop 2 ตัว (IC 7474) โดยต่อ $\bar{Q}_0$ เข้า $D_0$ และนำ $Q_0$ ต่อเข้าขา $CLK_1$ ของบิตที่สอง
**Inputs:** CLK, CLR_N
**Outputs:** Q0, Q1
**Gate Type:** D Flip-Flop (IC 7474)

**Body (optional):** สัญญาณนาฬิกา $CLK$ ขับบิต $Q_0$ เมื่อ $Q_0$ เปลี่ยนสภาวะขอบขาขึ้นจะขับบิต $Q_1$ ต่อเป็นทอดๆ ทำให้ได้ลำดับการนับเลข 2 บิตสมบูรณ์

#### 27.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7474 / 7493
**Instructions:**
- ป้อนสภาวะ รีเซ็ต CLR_N=0 เพื่อให้ $Q_1Q_0 = 00$
- เปิด CLR_N=1 แล้วส่งสัญญาณ Pulse ที่ CLK ทีละครั้ง เพื่อสังเกตลำดับการนับ $00 \rightarrow 01 \rightarrow 10 \rightarrow 11 \rightarrow 00$

**Verification Text:** ตรวจสอบวงจรนับ 2 บิตในการนับเรียงลำดับสภาวะฐานสอง $00, 01, 10, 11$ ครบถ้วน

**Truth Table:**
- CLR_N=0, CLK=0 --> Q1=0, Q0=0
- CLR_N=1, CLK=EDGE_RISING --> Q1=0, Q0=1
- CLR_N=1, CLK=EDGE_RISING --> Q1=1, Q0=0
- CLR_N=1, CLK=EDGE_RISING --> Q1=1, Q0=1
- CLR_N=1, CLK=EDGE_RISING --> Q1=0, Q0=0

#### 27.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจการทำงานของ 2-Bit Asynchronous Binary Counter ในการนับจำนวนและสลับสภาวะลอจิกดิจิทัลเรียบร้อยแล้ว