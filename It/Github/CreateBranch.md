---
title: ایجاد و استفاده از Branch در گیت هاب 
author: محمد رضا کریمی  
description: هنگامی که شما یک branch از روی master branch ایجاد میکنید در واقع یک کپی از master branch در  لحظه میسازید.همچنین  وقتی که شما روی branch خود کار میکنید و افراد دیگر روی master branch تغییراتی را ایجاد میکنند، شما میتوانید آن تغییرات را نیز دریافت کنید.
dateModified: 2019/02/13  
datePublished: 2019/02/13  
uid: It/Github/CreateBranch  
---

Branching یک راه برای کار کردن روی ورژن های مختلف یک repository در یک زمان است.
به صورت پیش فرض repository شما یک branch با نام master دارد که به عنوان branch اصلی در نظر گرفته میشود.
از branch ها برای آزمایش و ایجاد تغییرات قبل از commit کردن آن تغییرات روی master branch استفاده میشود.

هنگامی که شما یک branch از روی master branch ایجاد میکنید در واقع یک کپی از master branch در  لحظه میسازید و همچنین  وقتی که شما روی branch خود کار میکنید و افراد دیگر روی master branch تغییراتی را ایجاد میکنند، شما میتوانید آن تغییرات را نیز دریافت کنید.

در دیاگرام زیر میبینیم:
* master branch
* یک branch جدید به اسم feature
* مسیری که feature branch از ایجاد تا merge شدن با master branch طی میکند

![ایجاد branch](./CreateBranch/branching.png)

تا به حال پیش آمده که چندین ورژن از یک فایل را ذخیره کنید؟ مانند فایل های زیر:
* story.txt
* story-joe-edit.txt
* story-joe-edit-reviewed.txt

Branch ها اهدافی مشابه این را در repository دنبال میکنند.

در github، توسعه دهندگان، نویسندگان و طراحان برای، نگهداری، رفع ایرادات و یا کار کردن روی یک ویژگی، از branch استفاده میکنند تا آن ها را از master branch جدا کنند. زمانیکه تغییرات نهایی میشود آن branch را با master branch، ادغام (merge) میکنند.

برای ایجاد یک branch جدید:
1. بروید به repository که ایجاد کردید
2. در قسمت بالای لیست فایل ها، روی branch: master کلیک کنید
3. در کادری که نمایش داده میشود نام branch جدید را وارد کنید، برای مثال readme-edits
4. بر روی باکس آبی رنگ، Create branch کلیک کنید و یا 'Enter' بزنید

![ایجاد branch جدید](./CreateBranch/readme-edits.gif)

حالا شما دو branch با نام های، master و readme-edits دارید. آنها دقیقا شبیه هم هستند. در گام بعدی ما میخواهیم تغییراتی روی branch .جدید ایجاد کنیم
