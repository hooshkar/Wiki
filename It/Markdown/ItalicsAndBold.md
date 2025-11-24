---
title: Italic و Bold در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: Italic و Bold دو عنصر اساسی در قالب بندی متن به شمار می روند و در ایجاد ظاهر مناسب و کاربردی بسیار مهم است که انجام دادن آن در مارک داون Bold کردن و یا Italic کردن متن به سادگی امکان پذیر است. 
dateModified: 2025/11/24 
datePublished: 2018/05/16  
uid: It/Markdown/ItalicsAndBold  
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

_Italic_ و **Bold** دو عنصر اساسی در قالب بندی متن به شمار می روند. در مارک داون Bold کردن و یا Italic کردن متن به سادگی امکان پذیر است.



### ایتالیک (_Italic_) در مارک داون

برای _Italic_ کردن متن در مارک دوان (Markdown)،  کافیست آن متن را بین دو علامت `(_)` قرار دهید.

مثال:

```
_Italic کردن متن در مارک دوان (Markdown) بسیار ساده است._
```

خروجی:

_Italic کردن متن در مارک دوان (Markdown) بسیار ساده است._



### متن بولد (**Bold**) در مارک داون

Bold کردن متن هم مانند Italic بسیار ساده است. برای Bold کردن متن آن را بین دو علامت `(**)` قرار دهید.

مثال:

```
**Bold کردن متن در مارک دوان (Markdown) بسیار ساده است.**
```

خروجی:

**Bold کردن متن در مارک دوان (Markdown) بسیار ساده است.**



### خط کشیدن روی نوشته در مارک داون

 شما میتوانید به سادگی روی متنی که نوشتید خط بکشید. برای این کار از علامت `~~` قرار می دهیم.

مثال:

```
~~نوشتن با استفاده از مارک دوان (Markdown) بسیار سخت است.~~
```

خروجی:

~~نوشتن با استفاده از مارک دوان (Markdown) بسیار سخت است.~~


همچنین شما میتوانید از این عناصر در یک خط استفاده کنید و یا آنها را با هم ترکیب کنید.

مثال:

```
نوشتن با _استفاده_ از **مارک دوان (Markdown)** بسیار ساده است.
```

خروجی:

نوشتن با _استفاده_ از **مارک دوان (Markdown)** بسیار ساده است.

مثال:

```
_**مارک دوان (Markdown)**_
```

خروجی:

_**مارک دوان (Markdown)**_

حالا شما نحوه Bold و Italic کردن متن را در مارک دوان (Markdown) یاد گرفتید.


[ایتالیک (Italic) در مارک داون]: #ایتالیک-italic-در-مارک-داون
[متن بولد (Bold) در مارک داون]: #متن-بولد-bold-در-مارک-داون
[خط کشیدن روی نوشته در مارک داون]: #خط-کشیدن-روی-نوشته-در-مارک-داون