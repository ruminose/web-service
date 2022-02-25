ทดสอบเขียน Webservice เขียนข้อมูลลงเก็บไว้ใน Mysql

รันคอนโซล
![1645808454848](https://user-images.githubusercontent.com/84636543/155758948-42ecb92a-1842-463d-b106-6aa4eec09b80.jpg)
ครีเอทดาต้าเบสที่จะใช้บันทึกข้อมูลลง
![1645817366934](https://user-images.githubusercontent.com/84636543/155779578-65db8375-4738-41e9-ada7-148d361b41c5.jpg)
จากนั้นรัน Springboot
![1645817100716](https://user-images.githubusercontent.com/84636543/155780188-04e60f18-fe26-49c8-9081-e985bd8b63ab.jpg)
ลองเขียน RequestMapping ทดสอบดูว่า Springboot ศามารถรันได้ตามปกติหรือไม่
![1645817072190](https://user-images.githubusercontent.com/84636543/155781001-e98b365a-4a7b-4f79-801c-1585f97012c8.jpg)
จากนั้นสร้างคลาสไว้เก็บข้อมูลที่ต้องการจะบันทึกลง Mysql จากนั้นอ้างอิง Main จาก Persistence ที่กำหนดค่าไว้จาก Mysql ที่สร้างยูสเซอร์ขึ้นมาแล้วแกรนข้อมูลไปเก็บไว้ในอีกส่วนนึง
ทดสอบรัน Try {} Catch ไว้สำรองด้วยเผื่อมี Error จะได้ Thorw ออกไปแสดงได้ ถ้าข้อมูลบันทึกเข้าดาต้าเบสปกติ ให้ Springboot คืนสถานะ "Ok" ออกมา
![1645817161366](https://user-images.githubusercontent.com/84636543/155783795-991aedee-1d67-4f4c-9b77-70294f10782a.jpg)
จากนั้นลองเข้าไปใน Mysql และเรียกดูข้อมูลถ้ารันสปริงบูทได้ตามปกติและไม่ผิดพลาดตรงไหนข้อมูลจะขึ้นโชวในเทบิ้ลเรียบร้อย ทุกครั้งที่มีการรันสปริงบูทเข้าไปจะบันทึกข้อมูลใหม่เข้าไป 1 ครั้งเสมอ
![1645817200441](https://user-images.githubusercontent.com/84636543/155784000-7d71fc1c-dbc7-46c1-a5e8-57fd917f15cb.jpg)

จบการ Insert data from SpringBoot to Mysql.
