---
title: ایجاد و استفاده از Branch در گیت هاب
author: محمد رضا کریمی
description: هنگامی که شما یک branch از روی master branch ایجاد میکنید در واقع یک کپی از master branch در  لحظه میسازید.همچنین  وقتی که شما روی branch خود کار میکنید و افراد دیگر روی master branch تغییراتی را ایجاد میکنند، شما میتوانید آن تغییرات را نیز دریافت کنید.
dateModified: 2023/08/13
datePublished: 2019/02/13
uid: It/SourceControl/Github/CreateBranch
---

Branching یک راه برای کار کردن روی ورژن های مختلف یک Repository در یک زمان است.
به صورت پیش فرض repository شما یک branch با نام Master دارد که به عنوان branch اصلی در نظر گرفته م یشود.
از branch ها برای آزمایش و ایجاد تغییرات قبل از commit کردن آن تغییرات روی master branch استفاده می شود.

هنگامی که شما یک branch از روی master branch ایجاد می کنید در واقع یک کپی از master branch در  لحظه می سازید و همچنین  وقتی که شما روی branch خود کار می کنید و افراد دیگر روی master branch تغییراتی را ایجاد می کنند، شما می توانید آن تغییرات را نیز دریافت کنید.

### در دیاگرام زیر می بینیم:

* master branch
* یک branch جدید به اسم feature
* مسیری که feature branch از ایجاد تا merge شدن با master branch طی می کند

![ایجاد branch](./Images/branching.webp)

تا به حال پیش آمده که چندین ورژن از یک فایل را ذخیره کنید؟ مانند فایل های زیر:
* story.txt
* story-joe-edit.txt
* story-joe-edit-reviewed.txt

Branch ها اهدافی مشابه این را در repository دنبال میکنند.

در github، توسعه دهندگان، نویسندگان و طراحان برای، نگهداری، رفع ایرادات و یا کار کردن روی یک ویژگی، از branch استفاده می کنند تا آن ها را از master branch جدا کنند. زمانیکه تغییرات نهایی می شود آن branch را با master branch، ادغام (merge) می کنند.

### برای ایجاد یک branch جدید:

1. بروید به repository که ایجاد کردید
2. در قسمت بالای لیست فایل ها، روی branch: master کلیک کنید
3. در کادری که نمایش داده می شود نام branch جدید را وارد کنید، برای مثال readme-edits
4. بر روی باکس آبی رنگ، Create branch کلیک کنید و یا 'Enter' بزنید

![ایجاد branch جدید](./Images/readme-edits.gif)

حالا شما دو branch با نام های، master و readme-edits دارید. آنها دقیقا شبیه هم هستند. در گام بعدی ما می خواهیم تغییراتی روی branch جدید ایجاد کنیم.
