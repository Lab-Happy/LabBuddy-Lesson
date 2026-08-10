# ลำดับงาน

1. Fork repo นี้
2. Clone ไปที่เครื่อง
3. เปิดไฟล์ ในโฟลเดอร์ IC-Test ด้วย Lesson Authoring 

http://172.104.42.221:5050/lesson-editor

	เช่น IC_7404_Lesson

![960](image1.png)

1. ตรวจสอบชื่อไฟล์และองค์ประกอบในหน้า COVER


![960](Image2.png)



5. ตรวจสอบองค์ประกอบและรายละเอียดในหน้า THEORY

![960](Image3.png)


6. ตรวจสอบองค์ประกอบและรายละเอียดในหน้า CIRCUIT

![960](image4.png)

6.1 เช็คจำนวน port  ว่าตรงไหม เช่น AND gate 2-inputs จำนวน 4 ตัว ต้องมี  INPUT = 8, OUTPUT = 4 

 ![960](image4-1.png)

7. ตรวจสอบหน้า verify 

![960](Image5.png)

7.1 วิเคราะห์ truth table  สำหรับการตรวจสอบไอซี
หมายเหตุ ในขั้นนี้ เราจะตรวจสอบเฉพาะลอจิกที่ไม่ซ้ำกันและให้ผลการวัดเพื่อตรวจสอบเท่านั้น ไม่ได้ทดสอบทั้งหมด 

![986](Image6.png)


8. ตรวจสอบหน้า SUMMARY

![983](image7.png)

ตรวจให้ครบทุกใบงาน แล้วใส่ผลไว้ใน  [Issues #1](https://github.com/Lab-Happy/LabBuddy-Lesson/issues/1)