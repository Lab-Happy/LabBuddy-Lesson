# ลำดับงาน

1. Fork repo นี้
2. Clone ไปที่เครื่อง
3. เปิดไฟล์ ในโฟลเดอร์ IC-Test ด้วย Lesson Authoring 

http://172.104.42.221:5050/lesson-editor

	เช่น IC_7404_Lesson

![alt text|951](image1.png)

1. ตรวจสอบชื่อไฟล์และองค์ประกอบในหน้า COVER

![[Image2.png|950]]


5. ตรวจสอบองค์ประกอบและรายละเอียดในหน้า THEORY

![[Image3.png|953]]

6. ตรวจสอบองค์ประกอบและรายละเอียดในหน้า CIRCUIT
![[image4.png|952]]

6.1 เช็คจำนวน port  ว่าตรงไหม เช่น AND gate 2-inputs จำนวน 4 ตัว ต้องมี  INPUT = 8, OUTPUT = 4 

![[image4-1.png|961]]

7. ตรวจสอบหน้า verify 

![[Image5.png|964]]

7.1 วิเคราะห์ truth table  สำหรับการตรวจสอบไอซี
หมายเหตุ ในขั้นนี้ เราจะตรวจสอบเฉพาะลอจิกที่ไม่ซ้ำกันและให้ผลการวัดเพื่อตรวจสอบเท่านั้น ไม่ได้ทดสอบทั้งหมด 
 
![[Pasted image 20260811061234.png|967]]


8. ตรวจสอบหน้า SUMMARY
![[Pasted image 20260811061414.png|986]]



ตรวจให้ครบทุกใบงาน แล้วใส่ผลไว้ใน  [Issues #1](https://github.com/Lab-Happy/LabBuddy-Lesson/issues/1)