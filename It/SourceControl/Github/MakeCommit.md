---
title: کار روی Branch جدید و ایجاد Commit در GitHub
author: محمد رضا کریمی
description: در github، به ذخیره کردن تغییرات، Commit میگویند. هر commit شامل یک پیام است که توضیح میدهید چرا این تغییرات صورت گرفته است. دیگر همکاران شما با خواندن این پیام متوجه میشوند که شما چه کاری انجام داده اید.
dateModified: 2025/12/10
datePublished: 2019/02/13
uid: It/SourceControl/Github/MakeCommit
---

<style>
/* -----------------------
   تنظیمات کلی متن
-------------------------*/
body, .faq-block, p, li, td, th {
  font-size: 13px !important;
  line-height: 22px;
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
  margin-bottom: 2px;
}

/* -----------------------
   لینک‌ها
-------------------------*/

a {
  font-size: 13px !important;
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
  background-color: #e9f4ff; /* آبی خیلی کم‌رنگ */
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
  margin-top: 10px !important;
}

</style>

اکنون که یک **Branch** جدید به نام `readme-edits` ایجاد کرده‌اید، زمان آن رسیده که روی این **Branch** کار کنید. این **Branch** در حال حاضر یک کپی از **Master Branch** است. تغییرات جدیدی را روی آن اعمال خواهیم کرد.

## Commit: ذخیره تغییرات در GitHub
در GitHub، ذخیره تغییرات **Commit** نامیده می‌شود. هر **Commit** شامل یک پیام است که توضیح می‌دهد چرا تغییرات انجام شده‌اند. این پیام به شما و همکارانتان کمک می‌کند تا از هدف تغییرات و منطق پشت آن‌ها مطلع شوید.

### مراحل ایجاد تغییر و Commit کردن آن
برای ایجاد تغییرات در فایل **README.md** و ثبت آن‌ها به صورت **Commit**، مراحل زیر را دنبال کنید:

1. **باز کردن فایل**  
   - به `readme-edits Branch` بروید.  
   - روی فایل `README.md` کلیک کنید.

2. **ویرایش فایل**  
   - روی آیکن مداد که در بالای سمت راست صفحه قرار دارد، کلیک کنید.  
   - ویرایشگر (Editor) باز خواهد شد. در این بخش، اطلاعات جدیدی درباره پروژه بنویسید یا تغییرات دلخواه خود را اعمال کنید.

3. **نوشتن پیام Commit**  
   - در بخش پایینی ویرایشگر، یک پیام توضیحی بنویسید.  
   - پیام باید به‌صورت خلاصه و روشن توضیح دهد که چه تغییراتی اعمال شده و دلیل آن چیست. برای مثال:  
     - "اضافه کردن توضیحات پروژه به README"  
     - "اصلاح ساختار توضیحات پروژه"

4. **ثبت تغییرات**  
   - روی دکمه **Commit changes** کلیک کنید.

![ایجاد تغییر و Commit](./Images/commit.webp)

### نتیجه تغییرات
این تغییرات تنها در `readme-edits Branch` اعمال خواهند شد. `Master Branch` همچنان بدون تغییر باقی می‌ماند. اکنون، **readme-edits Branch** محتوایی دارد که با **Master Branch** متفاوت است. این تفاوت نشان می‌دهد که تغییرات شما در محیطی جداگانه نگهداری می‌شوند.

---

### مزیت استفاده از Commit‌ها
1. ثبت تغییرات به همراه توضیحات واضح.
2. امکان بازگشت به نسخه‌های قبلی در صورت نیاز.
3. بهبود شفافیت و همکاری در پروژه‌های تیمی.

در مرحله بعد، می‌توانید این تغییرات را با **Master Branch** ادغام (Merge) کنید. این کار با استفاده از یک **Pull Request** انجام خواهد شد.