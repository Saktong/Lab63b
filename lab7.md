# การทดลองที่ 7 เรื่องการใช้งาน Microcontroller โดยใช้สัญญาณ Analog OutPut PWM ควบคุมความสว่าง หรี่ไฟ หลอดไฟ LED

## วัตถุประสงค์

1. เพื่อทำการศึกษาเกี่ยวกับการเขียนโปรแกรม

2. เพื่อสามารถนำโปรแกรมที่เขียนไปประยุกต์ใช้ได้

## อุปกรณ์ที่ใช้

1. Microcontroller

2. LED สีแดง 5 ดวง

3. Resistor

4. สายไฟ

5. บอร์ดทดลอง

## ศึกษาข้อมูลเบื้องต้น

* การใช้งาน platformio https://platformio.org/

* การเริ่มเขียนโปรแกรมภาษา C https://benzneststudios.com/blog/c-programming/c-programming-basic-1/

* เรียนรู้ ESP-01   https://docs.platformio.org/en/latest/boards/espressif8266/esp01_1m.html

* การต่อวงจร Microcontroller และการเขียนโปรแกรมควบคุมเบื้องต้น https://learninginventions.org/?page_id=2198

* สอนต่อวงจรและวิธีทำ https://www.myarduino.net/article/88/%E0%B8%AA%E0%B8%AD%E0%B8%99%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99-arduino-%E0%B8%AA%E0%B8%B1%E0%B8%8D%E0%B8%8D%E0%B8%B2%E0%B8%93-analog-output-pwm-%E0%B8%84%E0%B8%A7%E0%B8%9A%E0%B8%84%E0%B8%B8%E0%B8%A1%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%AA%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87-%E0%B8%AB%E0%B8%A3%E0%B8%B5%E0%B9%88%E0%B9%84%E0%B8%9F-%E0%B8%AB%E0%B8%A5%E0%B8%AD%E0%B8%94%E0%B9%84%E0%B8%9F-led

## วิธีทำการทดลอง

1. ต่อหลอดไฟเข้ากับ Microcontroller

![image](https://user-images.githubusercontent.com/80880340/113245510-536ecf80-92e1-11eb-88dc-2880ab0f2024.png)

2. อัพโหลดโค้ดตามด้านล่าง

https://www.myarduino.net/article/88/%E0%B8%AA%E0%B8%AD%E0%B8%99%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99-arduino-%E0%B8%AA%E0%B8%B1%E0%B8%8D%E0%B8%8D%E0%B8%B2%E0%B8%93-analog-output-pwm-%E0%B8%84%E0%B8%A7%E0%B8%9A%E0%B8%84%E0%B8%B8%E0%B8%A1%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%AA%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87-%E0%B8%AB%E0%B8%A3%E0%B8%B5%E0%B9%88%E0%B9%84%E0%B8%9F-%E0%B8%AB%E0%B8%A5%E0%B8%AD%E0%B8%94%E0%B9%84%E0%B8%9F-led

3. กำหนดสัญญาณ PWM ในช่วง 0-255  ค่า 0 จะเท่ากับ 0v ค่า 255 จะเท่ากับ 5v

https://www.myarduino.net/article/88/%E0%B8%AA%E0%B8%AD%E0%B8%99%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99-arduino-%E0%B8%AA%E0%B8%B1%E0%B8%8D%E0%B8%8D%E0%B8%B2%E0%B8%93-analog-output-pwm-%E0%B8%84%E0%B8%A7%E0%B8%9A%E0%B8%84%E0%B8%B8%E0%B8%A1%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%AA%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87-%E0%B8%AB%E0%B8%A3%E0%B8%B5%E0%B9%88%E0%B9%84%E0%B8%9F-%E0%B8%AB%E0%B8%A5%E0%B8%AD%E0%B8%94%E0%B9%84%E0%B8%9F-led

4. จากตัวอย่างโค้ดจะเห็นว่า ไฟจะค่อยๆสว่างและค่อยๆหรี่จนดับลงตามรูป

https://www.myarduino.net/article/88/%E0%B8%AA%E0%B8%AD%E0%B8%99%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99-arduino-%E0%B8%AA%E0%B8%B1%E0%B8%8D%E0%B8%8D%E0%B8%B2%E0%B8%93-analog-output-pwm-%E0%B8%84%E0%B8%A7%E0%B8%9A%E0%B8%84%E0%B8%B8%E0%B8%A1%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%AA%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87-%E0%B8%AB%E0%B8%A3%E0%B8%B5%E0%B9%88%E0%B9%84%E0%B8%9F-%E0%B8%AB%E0%B8%A5%E0%B8%AD%E0%B8%94%E0%B9%84%E0%B8%9F-led

https://www.myarduino.net/article/88/%E0%B8%AA%E0%B8%AD%E0%B8%99%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99-arduino-%E0%B8%AA%E0%B8%B1%E0%B8%8D%E0%B8%8D%E0%B8%B2%E0%B8%93-analog-output-pwm-%E0%B8%84%E0%B8%A7%E0%B8%9A%E0%B8%84%E0%B8%B8%E0%B8%A1%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%AA%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87-%E0%B8%AB%E0%B8%A3%E0%B8%B5%E0%B9%88%E0%B9%84%E0%B8%9F-%E0%B8%AB%E0%B8%A5%E0%B8%AD%E0%B8%94%E0%B9%84%E0%B8%9F-led

5. ในโค้ดตัวอย่างจะใช้ for วนลูปค่อยๆประความสว่าง ค่าจะ เพิ่ม และ ลดลง ที่ละ 1

https://www.myarduino.net/article/88/%E0%B8%AA%E0%B8%AD%E0%B8%99%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99-arduino-%E0%B8%AA%E0%B8%B1%E0%B8%8D%E0%B8%8D%E0%B8%B2%E0%B8%93-analog-output-pwm-%E0%B8%84%E0%B8%A7%E0%B8%9A%E0%B8%84%E0%B8%B8%E0%B8%A1%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%AA%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87-%E0%B8%AB%E0%B8%A3%E0%B8%B5%E0%B9%88%E0%B9%84%E0%B8%9F-%E0%B8%AB%E0%B8%A5%E0%B8%AD%E0%B8%94%E0%B9%84%E0%B8%9F-led

 ## การบันทึกผลการทดลอง

 จากการทดลองพบว่าหากเขียนโปรแกรมถูกจะได้ว่า ไฟจะค่อยๆสว่างและจะค่อยๆหรี่จนดับลงไปตามสัญญาณ PWM
 
 ## อภิปรายผลการทดลอง
 
 เนื่องจากไม่ได้ทำการทดลองเองจริงๆ และเป็นเพียงการค้นหาข้อมูลจากทางอินเทอร์เน็ต จึงทำให้ไม่สามารถเห็นภาพโดยรวมได้ 
  หากเป็นไปได้อยากทำการทดลองที่คณะอีกรอบนึง
 
 ## คำถามหลังการทดลอง
 
 Q:หากต้องการให้โปรแกรมวนลูปต้องใช้คำสั่งใด
 
 A:ใช้คำสั่ง for
