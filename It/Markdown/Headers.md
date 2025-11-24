---
title: سرفصل‌ها در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: سرفصل یا تیتر اغلب در وب سایت‌ها، مقالات، مجلات و یادداشت‌ها مورد استفاده قرار می گیرد تا کاربر را به یک بخش خاص متوجه کند. همانطور که از نام آن پیداست، مانند عنوان در بخش های بالا قرار میگیرد.
dateModified: 2025/11/24 
datePublished: 2018/05/16  
uid: It/Markdown/Headers  
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

در این بخش به سراغ یکی دیگر از قرارداد‌های قالب بندی می رویم: Heading (سرفصل)

سرفصل یا تیتر اغلب در وب سایت‌ها، مقالات، مجلات و یادداشت‌ها مورد استفاده قرار می گیرد تا کاربر را به یک بخش خاص متوجه کند. همانطور که از نام آن پیداست، مانند عنوان در بخش های بالا قرار می گیرد.

شش نوع سرفصل یا تیتر در اندازه‌های مختلف وجود دارد. برای تبدیل یک عبارت به سرفصل آن عبارت را با علامت `(#)` آغاز کنید. طبق ترتیب سرفصل‌ها تعداد علامت هشتک را افزایش دهید، مثلا برای سرفصل اول یک علامت و برای سرفصل زیر مجموعه این سرفصل دو علامت قرار دهید.

مانند:

```
# Header 1
## Header 1.1
### Header 1.1.1
#### Header 1.1.1.1
##### Header 1.1.1.1.1
###### Header 1.1.1.1.1.1
```

خروجی:

# Header 1
## Header 1.1
### Header 1.1.1
#### Header 1.1.1.1
##### Header 1.1.1.1.1
###### Header 1.1.1.1.1.1
