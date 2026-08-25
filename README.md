# Piyawut Boonpeng

**Senior Programmer · Full Stack (Laravel / React) · Enterprise integration**  
Bangkok · Open to full-time roles · Available within 30 days

[LinkedIn](https://www.linkedin.com/in/piyawut-boonpeng-513840429/) · piyawut.b@hotmail.com

I design and ship the **integration layer** between sales, warehouse, finance, banks, and retail partners — not only CRUD screens.

12 years in IT: manufacturing ERP (PowerBuilder / Oracle), then 5 years as Senior Programmer at **Saha Pathanapibul PCL** building REST APIs, ERP/WMS sync, bank bill payment, EDI, and a React operations console.

These pages are **case studies** of that work. They do not include employer source code, secrets, or production data. See [LEGAL.md](LEGAL.md).

## Focus

| | |
|---|---|
| **Roles** | Senior Full Stack · Senior Backend · Senior Programmer |
| **Backend** | PHP, Laravel 5.2 / 8 / 13, REST, OpenAPI, Sanctum, queues |
| **Frontend** | React 19, TypeScript, Vite, TanStack Query |
| **Data** | Oracle, MySQL, SQL, schema design |
| **Integration** | ERP (NetSuite / Odoo), WMS, bank H2H / QR, EDI, marketplaces |
| **Delivery** | Docker, GitLab CI, RBAC, audit, AI as a copilot with human review |

## Selected work

| | Problem | What I delivered |
|---|---------|------------------|
| [01 · Integration hub](case-studies/01-integration-hub.md) | Sales, ERP, warehouse, and partner files were disconnected | Laravel 13 hub: 70+ documented APIs, overnight ERP sync, EDI and supplier stock jobs, Docker CI |
| [02 · Ops console](case-studies/02-ops-console.md) | Operations needed CLI or database access to run jobs | React 19 + Laravel 13 BFF with project RBAC and operational UIs |
| [03 · Banking & finance APIs](case-studies/03-bank-payment.md) | Bank payments did not post cleanly into AR | Host-to-host inquiry/confirm, Thai QR pay-in slips, e-WHT, PDPA |
| [04 · Long-lived API hub](case-studies/04-legacy-api-hub.md) | Many clients still on older API versions | Versioned Laravel 5.2 APIs; Oracle / Odoo / WMS / marketplace bridges without breaking production |
| [05 · Plant ERP](case-studies/05-manufacturing-erp.md) | Factory processes needed software and specifications | PowerBuilder / Oracle ERP (FIFO, PO, BOM, MRP); later System Analyst (SRS, flows) |

## Architecture

Illustrative names only — not internal hostnames.

```
Field sales / portals ──┐
                        │
Ops console ────────────┼──► Integration hub ──► ERP
                        │                   ├──► WMS
                        │                   ├──► Bank bill payment
                        │                   └──► Partner / EDI files
```

Original demo apps (fake domain, written from scratch) are outlined in [demos/README.md](demos/README.md).

---

## ภาษาไทย

วิศวกรอาวุโส ประสบการณ์ 12 ปี ทำชั้นเชื่อมระบบองค์กรที่ บมจ. สหพัฒนพิบูล: Laravel, React, Oracle, ธนาคาร, EDI, WMS

เคสศึกษา: [01](case-studies/01-integration-hub.md) · [02](case-studies/02-ops-console.md) · [03](case-studies/03-bank-payment.md) · [04](case-studies/04-legacy-api-hub.md) · [05](case-studies/05-manufacturing-erp.md)
