# Text/CSV Viewer

## 📖 Overview 

โปรแกรม **Text/CSV Viewer** เป็นโปรแกรมที่พัฒนาด้วย **C# Windows Forms**
สำหรับอ่านและแสดงผลข้อมูลจากไฟล์ **Text (.txt)** และ **CSV (.csv)**

ใน Assignment นี้ ได้มีการพัฒนาโปรแกรมเพิ่มเติมให้สามารถรองรับการทำงานกับชุดข้อมูล MalwareBazaar ขนาดใหญ่ รวมถึงเพิ่มความสามารถในการโหลดข้อมูลเฉพาะช่วงและกรองข้อมูลตามประเภทไฟล์

---

## ✨ Features (ความสามารถของโปรแกรม)

- อ่านไฟล์ Text (.txt)
- อ่านไฟล์ CSV (.csv)
- เลือกไฟล์ผ่านปุ่ม **Browse**
- รองรับการโหลดข้อมูลขนาดใหญ่ (Large Data Handling)
- โหลดข้อมูลเฉพาะช่วง (Partial Loading) โดยกำหนด Start และ End
- กรองข้อมูลตาม **File Type Filtering**
- ตรวจสอบความถูกต้องของข้อมูลที่ผู้ใช้กรอก (Input Validation)

---

## 🚀 How to Use (วิธีใช้งาน)

1. เปิดโปรแกรม
2. กดปุ่ม **Browse** เพื่อเลือกไฟล์ CSV
3. กำหนดช่วงข้อมูลที่ต้องการ
   - **Start** = ลำดับเริ่มต้น
   - **End** = ลำดับสุดท้าย
4. หากต้องการกรองข้อมูล ให้กรอกชนิดไฟล์ในช่อง **File Type**
   - ตัวอย่าง
     - exe
     - elf
     - js
5. กดปุ่ม **Load CSV**
6. โปรแกรมจะแสดงผลข้อมูลตามช่วงและเงื่อนไขที่กำหนด

---

## 📂 Dataset (ชุดข้อมูล)

โปรแกรมนี้ใช้ข้อมูลจาก **MalwareBazaar** เพื่อการศึกษาและทดลองพัฒนาโปรแกรม

สำหรับการทดสอบ Assignment ได้ใช้

- MalwareBazaar Sample CSV
- MalwareBazaar Full CSV

> **หมายเหตุ**
>
> ไฟล์ Full Dataset ใช้สำหรับการทดสอบภายในเครื่องเท่านั้น และ **ไม่ได้อัปโหลดขึ้น GitHub** ตามข้อกำหนดของ Assignment

---

## 📌 Features Added in This Assignment (ฟังก์ชันที่เพิ่ม)

สำหรับ Assignment นี้ ได้เพิ่มความสามารถดังนี้

- ✅ Large Data Handling
- ✅ Partial Loading (Start–End)
- ✅ File Type Filtering
- ✅ Input Validation
- ✅ รองรับการใช้งานกับ MalwareBazaar Full Dataset