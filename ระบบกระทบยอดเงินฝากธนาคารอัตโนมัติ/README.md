# README — เปิดโปรเจกต์ BankReconciliation

## 1. สิ่งที่ต้องมีก่อนเปิดงาน

| รายการ | รายละเอียด |
|---|---|
| UiPath Studio | เวอร์ชัน 26.0.197.0 หรือใหม่กว่า |
| UiPath.Excel.Activities | เวอร์ชัน 3.5.3 |
| UiPath.System.Activities | เวอร์ชัน 26.6.1 |
| ไฟล์ข้อมูล | `CompanyLedger.xlsx` (Sheet ชื่อ `Ledger`) และ `BankStatement.xlsx` (Sheet ชื่อ `Statement`) |

> ถ้า UiPath Studio เป็นคนละเวอร์ชัน ระบบจะขึ้นแจ้งให้ Restore Dependencies ให้กด **Restore/Update** ตามที่ Studio แนะนำ ไม่ต้องกังวล

---

## 2. วิธีเปิดงาน

1. แตกไฟล์ ZIP ไปไว้ในโฟลเดอร์ที่ต้องการ (แนะนำ Path ภาษาอังกฤษ ไม่มีช่องว่าง)
2. เปิด **UiPath Studio**
3. เลือก **Open Project** → เลือกไฟล์ `project.json` ในโฟลเดอร์ `BankReconciliation`
4. รอให้ Studio โหลด Dependencies ให้ครบ
5. เปิดไฟล์ **Main.xaml**
6. แก้ **Workbook path** ของ Activity "Use Excel File" ทั้ง 3 จุด (CompanyLedger, BankStatement, Result) ให้ตรงกับตำแหน่งไฟล์จริงในเครื่องที่เปิดงาน แล้วจึงกด Run
