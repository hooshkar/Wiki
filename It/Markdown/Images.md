---
title: قرار دادن عکس در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: در مارک داون (Markdown) مانند لینک دو نوع عکس وجود دارد، و هر دو نوع به یک شکل دیده میشود. تنها تفاوت لینک و عکس در این است که عکس با علامت تعجب آغاز میشود.
dateModified: 2025/11/24 
datePublished: 2018/05/16  
uid: It/Markdown/Images  
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

اگر شما مرحله قبل یعنی قرار دادن لینک در مارک داون (Markdown) را یاد گرفته باشید، شما میتوانید عکس هم قرار دهید. نحوه قراردادن عکس بسیار شبیه لینک است.

در مارک داون (Markdown) مانند لینک دو نوع عکس وجود دارد، و هر دو نوع به یک شکل دیده میشود. تنها تفاوت لینک و عکس در این است که عکس با علامت تعجب آغاز میشود.

## تصویر درون خطی (Inline Iamge)

اولین نوع قرار دادن عکس در مارک داون (Markdown) Inline Iamge نام دارد.

مثال:
```
![لوگو یاراد](./Images/yarad.webp)
```

خروجی:

![لوگو یاراد](./Images/yarad.webp)

متن نوشته شده به عنوان alt روی عکس قرار میگرد تا اگر مسیر عکس درست نبود و یا عکس لود نشد، متن نوشته شود.

مثال:
```
![لوگو یاراد](./Images/mistake-address.webp)
```
## تصویر مرجع (Reference Image)

نوع دیگر قرار دادن عکس در مارک داون (Markdown)`Reference Image` نام دارد. این نوع مانند رفرنس لینک است. رفرنس عکس‌ها را تعریف میکنیم و به جای آدرس از آن استفاده میکنیم.

نحوه استفاده:
```
[image name]: image address

[image title][image name]
```

مثال:
```
[logo yarad]: ./Images/yarad.webp

![لوگو یاراد][logo yarad]
```

خروجی:

[logo yarad]: ./Images/yarad.webp

![لوگو یاراد][logo yarad]


[تصویر درون خطی (Inline Iamge)]: #تصویر-درون-خطی-inline-iamge
[تصویر مرجع (Reference Image)]: #تصویر-مرجع-reference-image