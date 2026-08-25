# เดโมที่เขียนใหม่เอง

อย่า copy โฟลเดอร์จาก Laragon/WAMP/XAMPP ของบริษัทมาวางที่นี่

สร้าง repo ย่อยทีละอันบน GitHub ส่วนตัวก็ได้

## 1) mini-integration-hub (แนะนำทำก่อน)

Laravel เล็ก ๆ โดเมน “ร้านค้าสมมติ”

- `POST /orders` บันทึกออเดอร์
- จองสต็อกในตาราง `inventory_reservations`
- คำสั่ง `orders:sync-erp --dry-run` ดันไปยัง mock HTTP ของ ERP
- อ่านไฟล์ CSV ตัวอย่างใน `samples/` แล้วขึ้น staging table
- Swagger ของเราเอง

ข้อมูลใน `samples/` ต้องเป็นของปลอม (SKU-001, คลัง A)

## 2) mini-ops-console

React + Laravel

- Login + role `admin` / `operator` / `viewer`
- หน้า list งานซิงก์จากตารางปลอม
- ปุ่ม “Force sync” ยิง mock ไม่ยิงระบบจริง

## 3) mini-biller-api

Inquiry / Confirm ด้วย JSON ที่เราออกแบบเอง  
อย่าตั้งชื่อฟิลด์ให้เหมือนเอกสารธนาคารที่เซ็นสัญญา

เมื่อทำเสร็จ ใส่ลิงก์ repo เดโมใน README หลักของพอร์ตโฟลิโอ
