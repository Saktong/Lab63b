# การทดลองที่6. การเขียนโปรแกรมสร้างไวไฟแอคเซสพอยต์ (Wifi AP)

## วัตถุประสงค์

* สามารถต่อไวไฟที่เราสร้างขึ้นมาเองได้จากโทรศัพท์มือถือ 

## อุปกรณ์ที่ใช้

1. ESP-01 (microcontrollor)

2. USB2Serial converter

3.serial port

## ศึกษาข้อมูลเบื้อต้น

1. การใช้งาน platformio https://platformio.org/

2. การเริ่มเขียนโปรแกรมภาษา C https://benzneststudios.com/blog/c-programming/c-programming-basic-1/

3. เรียนรู้ ESP-01 https://docs.platformio.org/en/latest/boards/espressif8266/esp01_1m.html

4. การต่อวงจร Microcontroller และการเขียนโปรแกรมควบคุมเบื้องต้น https://learninginventions.org/?page_id=2198

5. 06 run wiri AP https://www.youtube.com/watch?v=T26DVHePlTs

## วิธีการทำการทดลอง

1. เปิดโปรแกรม ตัวอย่างที่6 

2.เข้าไปตั้งค่าในคำสั่ง เช่น ชื่อwifi รหัสและ ip ต่าง ๆ

![image](https://user-images.githubusercontent.com/80880340/112411032-cced4780-8d4e-11eb-9413-a9a948a58414.png)

3. สร้าง access point โดยrun WiFi.softAP กำหนด ssid และ password 

![8](https://user-images.githubusercontent.com/80879653/112207571-e22c7e00-8c49-11eb-81d6-41c4e967b8ca.png)

4. pio run -t upload

![9](https://user-images.githubusercontent.com/80879653/112208035-739bf000-8c4a-11eb-8f27-6adedf3731ed.png)

5. กดปุ่ม set เพื่อ upload

![10](https://user-images.githubusercontent.com/80879653/112208088-86162980-8c4a-11eb-952d-fcc508dcd191.png)

6. pio device mornitor

![11](https://user-images.githubusercontent.com/80879653/112208315-cb3a5b80-8c4a-11eb-8569-fa84f6c5dadc.png)

7. ใช้คอมพิวเตอร์ชคการเชื่อมจากโทรศัพท์ค้นหาไวไฟจาก EPS-01

![12](https://user-images.githubusercontent.com/80879653/112208673-32581000-8c4b-11eb-8132-0b27191109b6.png)



## การบันทึกผลการทดลอง
