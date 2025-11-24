---
title: ادغام Branch‌ها، Merge کردن تغییرات در GitHub
author: محمد رضا کریمی
description: بعد از اتمام کار روی یک شاخه، لازم می‌شود که کدهای  شاخه (branch) مورد نظر با یک شاخه‌ی دیگر (معمولاً master) ترکیب شود. گاهی هم ممکن است تغییراتی که در شاخه‌ی سومی وجود دارد را وارد شاخه‌ای که درحال کار روی آن هستیم کنیم. در این مواقع باید از دستور merge استفاده کنیم. 
dateModified: 2025/11/24
datePublished: 2019/02/13
uid: It/SourceControl/Github/MergePullRequest
---

<style>
/* -----------------------
   تنظیمات کلی متن
-------------------------*/
body, .faq-block, p, li, td, th {
  font-size: 13px !important;
  line-height: 25px;
  color: #002145;
  margin: 0;
  padding: 0;
}

/* فاصله بین پاراگراف‌ها */
p + p {
  margin-top: 10px !important;
}

/* فاصله بین هر پاراگراف و هدینگ */
p + h1,
p + h2,
p + h3,
p + h4 {
  margin-top: 30px !important;
}

/* فاصله‌های قبل از هدینگ */
h1, h2, h3, h4 {
  margin-top: 30px !important;
  margin-bottom: 10px !important;
}

/* -----------------------
   تنظیم اندازه هدینگ‌ها
-------------------------*/
h1 {
  font-size: 18px !important;
}

h2 {
  font-size: 16px !important;
}

h3, h4 {
  font-size: 15px !important;
}

/* -----------------------
   لیست‌ها
-------------------------*/
ul li {
  font-size: 13px !important;
  margin-bottom: 10px;
}

/* -----------------------
   لینک‌ها
-------------------------*/
a {
  font-size: 13px !important;
  color: #0d6efd;
}

/* -----------------------
   متن‌های بولد
-------------------------*/
strong, b {
  font-size: 12.5px !important;
}

/* -----------------------
   FAQ و فهرست
-------------------------*/
.faq-block {
  padding: 0.5rem;
  margin-top: 0.5rem;
  color: #002145 !important;
  font-size: 13px !important;
}

.faq-block summary {
  cursor: pointer;
  color: #002145 !important;
  font-size: 13px !important;
}

/* -----------------------
   جدول‌ها
-------------------------*/
table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px !important;
  font-size: 12.5px !important;
}

th, td {
  padding: 0.6rem !important;
  border: 1px solid #dcdcdc;
  text-align: right !important;
  font-size: 12.5px !important;
}

thead tr {
  background-color: #eeeeff;
}

tbody tr:nth-child(even) {
  background-color: #fafaff;
}

/* -----------------------
   فاصله بیشتر بین بخش‌ها
-------------------------*/
blockquote.faq-block {
  margin-top: 20px !important;
}

</style>

اکنون که تغییرات لازم را در **readme-edits Branch** اعمال و Commit کرده‌اید، زمان آن رسیده که این تغییرات را با **Master Branch** ادغام (Merge) کنید. فرآیند Merge به شما کمک می‌کند که تغییرات نهایی را به **Branch اصلی** پروژه منتقل کنید.

## مراحل Merge کردن Branch‌ها

1. **ایجاد Pull Request**  
   - به **Repository** خود بروید.  
   - در بخش بالای صفحه، روی گزینه **Pull requests** کلیک کنید.  
   - روی دکمه **New pull request** کلیک کنید.  
   - تغییرات موجود در **readme-edits Branch** را مرور کنید و آن‌ها را با **Master Branch** مقایسه کنید.  
   - یک پیام توضیحی در مورد Pull Request بنویسید (مثلاً: "اضافه کردن تغییرات فایل README").  
   - روی دکمه **Create pull request** کلیک کنید.

2. **ادغام Pull Request**  
   - زمانی که آماده هستید، روی دکمه سبز رنگ **Merge pull request** کلیک کنید.

   ![merge pull request](./Images/merge-button.webp)

   - برای تأیید، روی **Confirm merge** کلیک کنید.  
   - اکنون تغییرات **readme-edits Branch** با **Master Branch** ادغام شده است.

3. **حذف Branch اضافی**  
   - برای پاک‌سازی و جلوگیری از سردرگمی، می‌توانید **readme-edits Branch** را حذف کنید.  
   - پس از ادغام، روی گزینه **Delete branch** کلیک کنید.

![delete branch](./Images/delete-button.webp)

### نتیجه
با انجام این مراحل:
- تغییرات نهایی شما اکنون در **Master Branch** اعمال شده‌اند.  
- **readme-edits Branch** دیگر نیازی ندارد و حذف شده است، اما تمامی تغییرات آن در تاریخچه **Master Branch** ذخیره شده‌اند.  

---

### **مزایای این فرآیند**
1. **تفکیک و تست تغییرات**: Branch‌ها به شما اجازه می‌دهند که تغییرات را به‌صورت جداگانه اعمال کنید.  
2. **پیشگیری از ایرادات**: ادغام تغییرات پس از بازبینی و تأیید، باعث کاهش خطاها می‌شود.  
3. **نظم و سازمان‌دهی**: حذف Branch‌های اضافی از شلوغی Repository جلوگیری می‌کند.

در این مرحله، شما موفق به مدیریت، ویرایش، و ادغام تغییرات پروژه خود شده‌اید!















