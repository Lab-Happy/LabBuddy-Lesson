### **Lab 26: D Flip-Flop (Edge-Triggered)** — วงจรฟลิปฟลอปทำงานด้วยขอบสัญญาณนาฬิกา

#### 26.1 **Cover Page**
**File name:** Lab_26_D_Flip-Flop_Edge-Triggered_circuit_Lesson
**Title:** D Flip-Flop Lesson
**Subtitle:** วงจรฟลิปฟลอปชนิด D ทำงานด้วยขอบสัญญาณนาฬิกา
**IC Label:** 7474

**Objectives:**
- เข้าใจความแตกต่างระหว่าง Latch (Level-Triggered) และ Flip-Flop (Edge-Triggered)
- เรียนรู้การบันทึกค่าข้อมูล $D$ เข้าเอาต์พุต $Q$ เฉพาะ ณ จังหวะขอบขาขึ้น (Positive Edge Triggered) ของสัญญาณนาฬิกา ($CLK$)
- ศึกษาการใช้งานขาสัญญาณบังคับ Preset ($\bar{PRE}$) และ Clear ($\bar{CLR}$)

#### 26.2 **Theory Page**
**Title:** ทฤษฎีพื้นฐาน
**Body:** D Flip-Flop จะทำการสุ่มวัดค่าและบันทึกสัญญาณ $D$ ออกเอาต์พุต $Q$ เฉพาะเมื่อเกิดขอบขาขึ้น (Rising Edge $\uparrow$) ของสัญญาณนาฬิกา $CLK$:
- ณ จังหวะ $CLK \uparrow$: $Q = D$
- ระหว่างสภาวะ $CLK = 0$ หรือ $CLK = 1$ คงที่: เอาต์พุต $Q$ จะถูกล็อกและไม่เปลี่ยนแปลงตาม $D$ (Hold)
- ขาบังคับพิเศษ $\bar{PRE}$ และ $\bar{CLR}$ เป็น Active-Low บังคับตั้งค่า $Q=1$ หรือ $Q=0$ โดยไม่สนใจสัญญาณนาฬิกา

#### 26.3 **Circuit Page**
**Title:** วงจรทดลอง
**Hint:** ใช้ IC 7474 (Dual D-Type Positive-Edge-Triggered Flip-Flops) ต่อสัญญาณ D และป้อนสวิตช์จรวดชั่วขณะ (Pulse Button) ที่ขา CLK
**Inputs:** D, CLK, PRE_N, CLR_N
**Outputs:** Q, Q_N
**Gate Type:** D Flip-Flop (IC 7474)

**Body (optional):** สัญญาณ D ถูกป้อนไว้ล่วงหน้า จากนั้นส่งสัญญาณ Pulse ขาขึ้นที่ CLK เพื่อย้ายข้อมูล D ไปยังเอาต์พุต Q

#### 26.4 **Verify Page**
**Title:** ตรวจสอบวงจร **IC:** 7474
**Instructions:**
- ตั้งค่า PRE_N=1, CLR_N=1 (ปิดการบังคับ)
- ป้อน D=1 แล้วกดสร้างขอบขาขึ้นที่ CLK ยืนยันว่า Q=1
- ป้อน D=0 แล้วกดสร้างขอบขาขึ้นที่ CLK ยืนยันว่า Q=0
- ทดสอบเปลี่ยน D โดยไม่กด CLK ยืนยันว่า Q ไม่เปลี่ยน

**Verification Text:** ตรวจสอบวงจร D Flip-Flop ในการย้ายข้อมูล D ไปยัง Q เฉพาะขอบขาขึ้นของ CLK

**Truth Table:**
- PRE_N=1, CLR_N=1, CLK=EDGE_RISING, D=0 --> Q=0, Q_N=1
- PRE_N=1, CLR_N=1, CLK=EDGE_RISING, D=1 --> Q=1, Q_N=0
- PRE_N=0, CLR_N=1, CLK=0, D=0 --> Q=1, Q_N=0
- PRE_N=1, CLR_N=0, CLK=0, D=0 --> Q=0, Q_N=1

#### 26.5 **Summary Page**
**Title:** สรุปผล
**Body:** สำเร็จแล้วครับ! ผู้เรียนเข้าใจหลักการทำงานของ D Flip-Flop แบบขอบสัญญาณนาฬิกาและการควบคุมสภาวะความจำเรียบร้อยแล้ว