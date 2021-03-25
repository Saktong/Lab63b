# การทดลองที่ 5 เรื่อง การเขียนโปรแกรมเชื่อมต่อไวไฟและเว็บเซอร์เวอร์

## วัตถุประสงค์

1. เพื่อเขียนโปรแกรมเชื่อมต่อไวไฟทำหน้าที่ทดสอบเว็บเบราเซอร์

2. เพื่อศึกษาระบบเครือข่ายอินเทอร์เน็ตเบื้องต้น

## อุปกรณ์ที่ใช้
1. ESP-01 (microcontrollor)
2. USB2Serial converter
3. serial port

## ศึกษาข้อมูลเบื้อต้น
1. การใช้งาน platformio https://platformio.org/
2. การเริ่มเขียนโปรแกรมภาษา C https://benzneststudios.com/blog/c-programming/c-programming-basic-1/
3. เรียนรู้ ESP-01 https://docs.platformio.org/en/latest/boards/espressif8266/esp01_1m.html
4. การต่อวงจร Microcontroller และการเขียนโปรแกรมควบคุมเบื้องต้น https://learninginventions.org/?page_id=2198
5. run wifi https://www.youtube.com/watch?v=VX-QNQcO-b4&feature=youtu.be

## วิธีการทำการทดลอง

1. เปิดตัวอย่างโปรแกรมที่5

2. ตั้งค่าโปรแกรมโดยทำการเชื่อมต่อwifi โดยป้อนชื่อwifiและรหัสผ่าน

![image](https://user-images.githubusercontent.com/80880340/112405002-04a2c200-8d44-11eb-86cc-6dff3a445803.png)

![image](https://user-images.githubusercontent.com/80880340/112405019-0d939380-8d44-11eb-81b9-46f920f60d00.png)

3. อัปโหลดโปรแกรมไว้ที่ microcotrollor โดยเสียบไปที่ USB2Serial converter และทำการกดปุ่ม เพื่ออัปโหลด

![4](https://user-images.githubusercontent.com/80879653/112204250-08e8b580-8c46-11eb-969f-2bdc316aab27.png)

![5 เสียบไมโคกับUSB2](https://user-images.githubusercontent.com/80879653/112204386-2f0e5580-8c46-11eb-9857-caf37a9c0e55.png)

4. ทดสอบโดย เข้า เวบเบราเซอร์

![7  ทดสอบไวไฟ](https://user-images.githubusercontent.com/80879653/112204496-4e0ce780-8c46-11eb-96d2-0a1b8319ae2e.png)

## การบันทึกผลการทดลอง

จากการเขียนโปรแกรม เมื่อแสดงผล จะแสดง IP address และเมื่อคัดลอกและนำไปเปิดบนเว็บบราวเซอร์ ก็จะแสดงผล Hello 1 โดยที่จะนับและเปรี่ยนตัวแปรไปเรื่อยๆ

## อภิปรายผลการทดลอง

จากการทดลองเขียนโปรแกรมสามารถสรุปได้ว่า เราสามาให้ microcontrollor เชื่อมต่อไวไฟ และเว็บเซิร์ฟเวอร์สามารถทำงานได้เหมือเซิร์ฟเวอร์ทั่วไป

## คำถามหลังการทดลอง

Q: ssid คืออะไร

A:คือชื่อของ network ที่ตั้งขึ้นมา โดยที่ทุกๆเครื่องในระบบจะต้องตั้งค่า ssid ค่าเดียวกัน
