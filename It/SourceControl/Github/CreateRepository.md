---
title: ایجاد و مدیریت Repository در GitHub، راهنمای گام به گام
author: محمد رضا کریمی
description: از repository معمولا برای مدیریت و سازمان دهی یک پروژه استفاده میشود. معادل فارسی repositoy، مخزن است، هر آنچه که پروژه ما به آن نیاز دارد از جمله پوشه ها (folders)، فایل ها (files)، تصاویر (images)، فیلم ها (videos) و...، در آن قرار میگیرد.
dateModified: 2025/12/10
datePublished: 2019/02/13
uid: It/SourceControl/Github/CreateRepository
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
  animation: colorRotate 4s linear infinite;
}

@keyframes colorRotate {
  0%   { color: #0d6efd; }
  25%  { color: #1ecbe1; }
  50%  { color: #00c37a; }
  75%  { color: #ff7f50; }
  100% { color: #0d6efd; }
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

از **repository** معمولاً برای مدیریت و سازماندهی یک پروژه استفاده می‌شود.

معادل فارسی **repository**، **مخزن** است. در این مخزن، هر آنچه که پروژه به آن نیاز دارد، از جمله پوشه‌ها (folders)، فایل‌ها (files)، تصاویر (images)، فیلم‌ها (videos) و ... قرار می‌گیرد.

یکی از نکات مهم در استفاده از GitHub این است که همیشه پروژه شما یک فایل **README** داشته باشد که در آن اطلاعاتی در مورد پروژه نوشته می‌شود. این فایل معمولاً به توضیح هدف پروژه، نحوه استفاده و دیگر اطلاعات مهم پروژه پرداخته و به دیگران کمک می‌کند تا بهتر با پروژه آشنا شوند.

در **GitHub** می‌توانید هنگام ایجاد یک repository جدید، فایل‌هایی مانند **README** و یا فایل **لایسنس** (License) را نیز به آن اضافه کنید. این کار به شما کمک می‌کند تا پروژه‌تان به‌خوبی مستند و در دسترس قرار گیرد.

## مراحل ایجاد یک repository در GitHub

1. در نوار بالای صفحه GitHub، در سمت راست کنار آیکون آواتار (Avatar)، بر روی آیکون **+** کلیک کنید و گزینه **<a href="https://github.com/new" target="_blank">New repository</a>** را انتخاب کنید.
   
2. در قسمت **Repository Name**، نام repository خود را که در اینجا **hello-world** است، وارد کنید.

3. یک توضیح کوتاه در مورد این پروژه بنویسید. این توضیحات می‌تواند شامل هدف پروژه، ویژگی‌های اصلی و دیگر اطلاعات مرتبط با پروژه باشد.

4. می‌توانید با انتخاب گزینه **Private** مخزن خود را از دید بقیه کاربران سایت مخفی کنید. در غیر این صورت، اگر گزینه **Public** را انتخاب کنید، دیگر کاربران می‌توانند مخزن شما و محتویات آن را مشاهده کنند.

5. گزینه **Initialize this repository with a README** را انتخاب کنید تا به مخزن شما یک فایل **README** اضافه شود. این فایل معمولاً اطلاعات اولیه در مورد پروژه را در خود جای می‌دهد و اولین قدم در مستندسازی پروژه است.

6. شما همچنین می‌توانید با اضافه کردن **لایسنس** (License) به مخزن خود، دیگران را در استفاده از محتویات مخزن محدود کنید. با انتخاب گزینه **Add a license** می‌توانید یکی از لایسنس‌های رایج را انتخاب کنید که تعیین می‌کند چه مجوزهایی برای استفاده از پروژه خود دارید.

7. برای ایجاد روی **Create Repository** کلیک کنید.

این مراحل به شما کمک می‌کند تا یک repository ساده و مرتب برای پروژه خود در GitHub ایجاد کنید که به راحتی می‌توانید محتویات پروژه‌تان را در آن نگهداری و به اشتراک بگذارید.

![ایجاد repository](./Images/create-new-repo.webp)