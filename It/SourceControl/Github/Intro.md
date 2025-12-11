---
title: آموزش GitHub ایجاد پروژه Hello World و مفاهیم پایه‌ای مدیریت کد
author: محمد رضا کریمی
description: گیت هاب (github) یک وب سایت برای نگهداری پروژه و همکاری است. شما میتوانید پروژه خود را روی این وب سایت قرار دهید و تغییرات خود را روی آن اعمال کنید و همچنین همکارانتان را به این پروژه اضافه کنید تا در هر جایی که هستند به آن دسترسی پیدا کنند.
dateModified: 2025/12/10
datePublished: 2019/02/13
uid: It/SourceControl/Github/Intro
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

یک چیز مرسوم در حوزه برنامه‌نویسی ایجاد پروژه‌های Hello World است.

هنگامی که شروع می‌کنیم به یادگیری یک زبان یا ابزار جدید، یک پروژه با نام Hello World ایجاد می‌کنیم. این پروژه یک تمرین بسیار ساده برای یادگیری مباحث اولیه است که به ما کمک می‌کند با محیط و مفاهیم اصلی آشنا شویم.

حال قصد داریم با GitHub آشنا شویم. بنابراین، ابتدا تلاش می‌کنیم تا یک پروژه به نام **HelloWorld** روی GitHub ایجاد کنیم.

**GitHub** یک وب‌سایت برای نگهداری پروژه‌ها و همکاری‌های تیمی است. شما می‌توانید پروژه خود را روی این وب‌سایت قرار دهید و تغییرات خود را بر روی آن اعمال کنید. همچنین، همکارانتان می‌توانند به پروژه شما دسترسی داشته باشند و در هر زمان و مکانی بر روی آن کار کنند.

در این آموزش، مفاهیم اساسی GitHub مانند **repositories**، **branches**، **commits** و **pull requests** را بررسی خواهیم کرد. 

اولین قدم، ایجاد یک repository با نام **Hello World** است که به شما این امکان را می‌دهد تا گردش کار یک pull request را یاد بگیرید. ما مراحل انجام این کار را به‌طور ساده و گام به گام توضیح خواهیم داد.

برای گذراندن این آموزش، شما تنها نیاز به یک <a href="https://github.com" target="_blank">اکانت github</a> و دسترسی به اینترنت دارید. در اینجا نیازی به نوشتن کد، کار با خط فرمان یا نصب Git نیست.

**مطالبی که در این آموزش یاد خواهید گرفت:**

* <a href="https://www.hooshkar.com/Wiki/Github/CreateRepository" target="_blank">ایجاد و استفاده از repository</a>

* <a href="https://www.hooshkar.com/Wiki/Github/CreateBranch" target="_blank">ایجاد و استفاده از Branch در گیت هاب</a>

* <a href="https://www.hooshkar.com/Wiki/Github/MakeCommit" target="_blank">تغییر یک فایل و فرستادن آن به github به عنوان یک commit</a>

* <a href="https://www.hooshkar.com/Wiki/Github/OpenPullRequest" target="_blank">باز کردن و ادغام (merge) یک pull request</a>

این آموزش به شما کمک می‌کند تا نحوه مدیریت پروژه‌های خود را در GitHub یاد بگیرید و ابزارهای پایه‌ای این پلتفرم را درک کنید.