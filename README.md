# การติดตั้งโปรแกรม สำหรับสร้าง ENV ให้กับ Program #
1. ต้องการ PHP เวอร์ชั่น 7.1.3 ขึ้นไป
2. ต้องการฐานข้อมูล (Database) ที่ทำงานด้วย MySQL
3. ต้องทำการติดตั้งโปรแกรม Composer เพื่อทำการ Compile File composer.json
4. ต้องทำการติดตั้งโปรแกรม NodeJS เพื่อทำการ Compile File package.json

# การติดตั้งโปรแกรม #
1. ทำการ Clone Project ลงมายังเครื่องใน Folder ที่ต้องการ
2. ใช้คำสั้ง $ composer install เพื่อติดตั้ง Package จากไฟล์ composer.json
3. ใช้คำสั่ง $ npm install เพื่อติดตั้ง Package จากไฟล์ package.json
4. ใข้คำสั้ง php artisan serv เพื่อทำการ Run Project และ ใช้คำสั่ง npm run dev หรือ npm run watch
   เพื่อทำการ Compile Javasctipt (VueJS Framework)
   
# การเชื่อมต่อฐานข้อมูล #
1. สร้างฐานข้อมูลชื่อ oam_db ในรูปแบบ utf8_general_ci
2. ใช้คำสั่ง php artisan key:generate เพื่อทำการ generate key ใหม่กับไฟล์ .env
3. Compile ฐานข้อมูลด้วยคำสั่ง php artisan migrate
4. ทำการทดสอบ Run โปรแกรมอีกครั้งด้วยคำสั่ง php artisan serv