---
title: Lists در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: این بخش آموزش در مورد لیست‌ها در مارک داون (Markdown) است. دو نوع لیست وجود دارد اولی لیست‌های نامرتب و دومی لیست‌های مرتب، که به آن‌ها لیست‌های با Bullet و لیست‌‌های با عدد نیز می‌گویند.
dateModified: 2025/11/24
datePublished: 2018/05/16  
uid: It/Markdown/Lists  
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

این بخش آموزش در مورد لیست‌ها در مارک داون (Markdown) است. دو نوع لیست وجود دارد اولی لیست‌های نامرتب و دومی لیست‌های مرتب، که به آن‌ها لیست‌های با Bullet و لیست‌‌های با عدد نیز می‌گویند.

## ایجاد لیست های نامرتب

برای ایجاد لیست‌های نامرتب در مارک داون (Markdown) فقط کافیست قبل از هر آیتم یک علامت `*` قرار دهید و همچنین هر آیتم از لیست باید در یک خط قرار گیرد.

مثال:

````
* Milk
* Eggs
* Salmon
* Butter
````

خروجی:

* Milk
* Eggs
* Salmon
* Butter

## ایجاد لیست های مرتب
برای ایجاد لیست‌های مرتب، باید به جای علامت `*`، علامت عدد قرار دهید.

مثال:

```
1. Crack three eggs over a bowl
2. Pour a gallon of milk into the bowl
3. Rub the salmon vigorously with butter
4. Drop the salmon into the egg-milk bowl
```

خروجی:

1. Crack three eggs over a bowl
2. Pour a gallon of milk into the bowl
3. Rub the salmon vigorously with butter
4. Drop the salmon into the egg-milk bowl

برای ایجاد فرزند برای هر آیتم از لیست کافیست که فرزند آنرا به اندازه یک تب جلوتر قرار دهید.

مثال:

```
* Tintin
    * A reporter
        * Has poofy orange hair
        * Friends with the world's most awesome dog
* Haddock
 * A sea captain
 * Has a fantastic beard
 * Loves whiskey
   * Possibly also scotch?
```

خروجی:

* Tintin
    * A reporter
        * Has poofy orange hair
        * Friends with the world's most awesome dog
* Haddock
    * A sea captain
    * Has a fantastic beard
    * Loves whiskey
        * Possibly also scotch? 

شما میتوانید در لیست‌ها از عناصر دیگر مارک داون (Markdown) نیز استفاده کنید.

مثال:

```
1. Crack three eggs over a bowl.

 Now, you're going to want to crack the eggs in such a way that you don't make a mess.

 If you _do_ make a mess, use a towel to clean it up!

2. Pour a gallon of milk into the bowl.

 Basically, take the same guidance as above: don't be messy, but if you are, clean it up!

3. Rub the salmon vigorously with butter.

   By "vigorous," we mean a strictly vertical motion. Julia Child once quipped:
   > Up and down and all around, that's how butter on salmon goes.
4. Drop the salmon into the egg-milk bowl.

   Here are some techniques on salmon-dropping:

   * Make sure no trout or children are present
   * Use both hands
   * Always have a towel nearby in case of messes
```

خروجی:

1. Crack three eggs over a bowl.

 Now, you're going to want to crack the eggs in such a way that you don't make a mess.

 If you _do_ make a mess, use a towel to clean it up!

2. Pour a gallon of milk into the bowl.

 Basically, take the same guidance as above: don't be messy, but if you are, clean it up!

3. Rub the salmon vigorously with butter.

   By "vigorous," we mean a strictly vertical motion. Julia Child once quipped:
   > Up and down and all around, that's how butter on salmon goes.
4. Drop the salmon into the egg-milk bowl.

   Here are some techniques on salmon-dropping:

   * Make sure no trout or children are present
   * Use both hands
   * Always have a towel nearby in case of messes

[ایجاد لیست های نامرتب]: #ایجاد-لیست-های-نامرتب
[ایجاد لیست های مرتب]: #ایجاد-لیست-های-مرتب