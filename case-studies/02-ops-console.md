# เคส 2 — Operations console (React + Laravel)

| | |
|---|---|
| **Role** | Primary author · greenfield · 2026 |
| **Stack** | React 19, TypeScript, Vite, TanStack Query, Laravel 13, Sanctum, Docker, MySQL |
| **For hiring** | Full-stack proof: RBAC, BFF, ops UX — no employer UI source |

## ปัญหา

งานซิงก์ แก้บิล และสร้างไฟล์ทำผ่าน CLI หรือฐานข้อมูลตรง  
หลายทีมใช้เครื่องมือคนละชุด ไม่มี RBAC รวม

## สิ่งที่ออกแบบ

- SPA + API แบบ BFF: ตรวจสิทธิ์ที่คอนโซล แล้วเรียกบริการภายใน
- RBAC แยกตามโปรเจกต์ (ทีมบิล, ทีมคลัง, ทีมซิงก์)
- ล็อกอินผูกพนักงานบริษัท, idle timeout, audit ปิดบังรหัสผ่าน/ข้อมูลส่วนบุคคล
- หน้าจอ: รายการงานซิงก์, บังคับซิงก์, แก้บิลโลจิสติกส์, สร้างไฟล์ส่งออก, เครื่องมือวินิจฉัย API

## ผล

ฝ่ายปฏิบัติการกดงานเองได้โดยไม่ต้องเข้าเซิร์ฟเวอร์  
โชว์ Full Stack จริง: UI + API + auth + deploy

## เดโมส่วนตัวที่อนุญาตให้มีโค้ด

แนวทางใน [demos/README.md](../demos/README.md) — แอปตัวอย่างแผงควบคุมงานซิงก์ด้วยข้อมูลปลอม (ยังไม่ได้ใส่ซอร์สใน repo นี้)
