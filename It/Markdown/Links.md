---
title: قرار دادن لینک در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: در این بخش از مارک داون با نحوه لینک دادن به وب سایت‌های دیگر آشنا میشویم. در مارک داون (Markdown) دو نوع لینک دادن وجود دارد، اما هر دو نوع به یک شکل دیده میشود.
dateModified: 2025/11/24 
datePublished: 2018/05/16  
uid: It/Markdown/Links  
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

در این بخش از مارک داون با نحوه لینک دادن به وب سایت‌های دیگر آشنا میشویم. در مارک داون (Markdown) دو نوع لینک دادن وجود دارد، اما هر دو نوع به یک شکل دیده میشود.

## لینک درون خطی (Inline Link)

اولین نوع لینک دادن، Inline Link نام دارد. برای ایجاد این نوع لینک متن لینک را در `[]`، و آدرس را در `()` قرار میدهیم.

مثال:

```
[وب سایت هوشکار](https://www.hooshkar.com)
```

خروجی:

[وب سایت هوشکار](https://www.hooshkar.com)

شما میتوانید متن لینک را بصورت Italic و یا Bold بنویسید.

مثال:

```
[_وب سایت هوشکار_](https://www.hooshkar.com)
[**وب سایت هوشکار**](https://www.hooshkar.com)
```

خروجی:

[_وب سایت هوشکار_](https://www.hooshkar.com)
[**وب سایت هوشکار**](https://www.hooshkar.com)

همچنین میتوانید درون سرفصل لینک را قرار دهید.

مثال:

```
### وب سایت شرکت  [هوشکار](https://www.hooshkar.com)
```

خروجی:

### وب سایت شرکت  [هوشکار](https://www.hooshkar.com)

## لینک مرجع (Reference Link)

نوع دیگر لینک‌ها در مارک داون (Markdown) Reference Link است، رفرنس لینک به این صورت است که برای آدرس یک نام مشخص میشود و بجای استفاده از آدرس از نام آن استفاده میشود. و اگر بخواهیم آدرس تغییر کند لازم نیست کل لینک‌ها را تغییر دهیم. برای استفاده از رفرنس لینک ابتدا باید برای آن آدرس یک اسم مشخص کنید و بعد از اسم آن استفاده کنید. بهتر است که رفرنس لینک‌ها را در ابتدا و یا انتهای فایل md تعریف کنید.

نحوه استفاده از رفرنس لینک‌ها:

```
[link name]: address

[link text][link name]

```

مثال:

```
[hooshkar]: https://www.hooshkar.com

[hooshkarpardaz][hooshkar]
[hoshkar][hooshkar]
```

خروجی:

[hooshkar]: https://www.hooshkar.com

[hooshkarpardaz][hooshkar]
[hoshkar][hooshkar]


[لینک درون خطی (Inline Link)]: #لینک-درون-خطی-inline-code
[لینک مرجع (Reference Link)]: #لینک-مرجع-reference-link