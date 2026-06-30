# Testing Report (รายงานการทดสอบ)

## Project (โครงการ)

Text/CSV Viewer

---

## Objective (วัตถุประสงค์)

เพื่อทดสอบว่าโปรแกรมสามารถทำงานได้ถูกต้องตามที่กำหนด ได้แก่

- โหลดไฟล์ CSV ขนาดใหญ่ (Large Data Handling)
- โหลดข้อมูลเฉพาะช่วง (Partial Loading)
- ค้นหาด้วย File Type Filtering
- ตรวจสอบความถูกต้องของข้อมูลที่ผู้ใช้กรอก (Input Validation)

---

## Test Cases (กรณีทดสอบ)

| Test ID | Feature | Input | Expected Result (ผลที่คาดหวัง) | Actual Result (ผลที่ได้) | Pass/Fail |
|---------|---------|-------|--------------------------------|--------------------------|-----------|
| TC01 | Partial Loading | Start = 1, End = 100 | แสดงข้อมูลลำดับที่ 1–100 | โปรแกรมแสดงข้อมูล 100 รายการถูกต้อง | Pass |
| TC02 | File Type Filter | File Type = exe | แสดงเฉพาะข้อมูลประเภท exe | โปรแกรมแสดงเฉพาะข้อมูล exe | Pass |
| TC03 | File Type Filter | File Type = elf | แสดงเฉพาะข้อมูลประเภท elf | โปรแกรมแสดงเฉพาะข้อมูล elf | Pass |
| TC04 | Invalid Range | Start = 100, End = 1 | โปรแกรมแจ้งเตือนช่วงข้อมูลไม่ถูกต้อง | โปรแกรมแสดงข้อความแจ้งเตือน | Pass |
| TC05 | No Matching Data | File Type = pdf | ไม่พบข้อมูลที่ตรงกับเงื่อนไข | โปรแกรมไม่แสดงข้อมูลที่ตรงเงื่อนไข | Pass |

---

## Test Environment (สภาพแวดล้อมในการทดสอบ)

- Operating System : Windows 10
- IDE : Visual Studio 2022
- Programming Language : C#
- Framework : Windows Forms
- Dataset : MalwareBazaar Full CSV

---

## Result Summary (สรุปผลการทดสอบ)

ผลการทดสอบพบว่า

- โปรแกรมสามารถโหลดไฟล์ CSV ขนาดใหญ่ได้
- โปรแกรมสามารถโหลดข้อมูลเฉพาะช่วง (Partial Loading) ได้ถูกต้อง
- โปรแกรมสามารถกรองข้อมูลตาม File Type ได้
- โปรแกรมสามารถตรวจสอบข้อมูลที่ผู้ใช้กรอกได้อย่างถูกต้อง
- การทำงานของโปรแกรมเป็นไปตามที่ออกแบบไว้

---

## Remarks (หมายเหตุ)

- ใช้ชุดข้อมูล MalwareBazaar Full CSV สำหรับการทดสอบ
- ชุดข้อมูลฉบับเต็มใช้สำหรับการทดสอบภายในเท่านั้น และไม่ได้อัปโหลดขึ้น GitHub ตามข้อกำหนดของ Assignment