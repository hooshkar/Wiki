---
title: نمایش کد در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: در مارک داون برای نمایش متن و یا بهتر است بگوییم نمایش کد، کافیست آن قطعه کد را بین دو علامت بک‌‌ تیک (`) قرار دهید. که به این نوع نمایش کد، Inline Code می‌گویند.
dateModified: 2025/12/10
datePublished: 2018/05/16  
uid: It/Markdown/CodeWriting  
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

## کد درون خطی (Inline Code)
برای نمایش متن و یا بهتر است بگوییم نمایش کد، کافیست آن قطعه کد را بین دو علامت بک‌‌ تیک (`) قرار دهید.که به این نوع نمایش کد، Inline Code می‌گویند.

مثال:

```
I think you should use an
`code here` element here instead
```

خروجی:

I think you should use an
`code here` element here instead

هرچیزی که داخل دو علامت بک تیک (`) قرار دهید به همان شکل نشان داده می شوند.

## بلاک کد

اگر شما قصد نمایش یک بلاک کد را دارید کافیست در ابتدا و انتهای آن، سه علامت بک تیک (`) قرار دهید.

مثال :

````
Some basic Git commands are:
```
git status
git add
git commit
```
````

خروجی:

Some basic Git commands are:
```
git status
git add
git commit
```
## نمایش کد به صورت رنگی
شما میتوانید زبان قطعه کد  را بنویسید تا با رنگ‌های بهتری نمایش داده شود.

مثال :

````
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
````

خروجی:

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

[کد درون خطی (Inline Code)]: #کد-درون-خطی-inline-code
[بلاک کد]: #بلاک-کد
[نمایش کد به صورت رنگی]: #نمایش-کد-به-صورت-رنگی