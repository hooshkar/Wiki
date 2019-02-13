---
title: قرار دادن لینک در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: آموزش قرار دادن لینک به صورت Inline Link و Refrence Link در مارک داون (Markdown)  
dateModified: 2018/05/16  
datePublished: 2018/05/16  
uid: It/Markdown/Links  
---

در این بخش با نحوه لینک دادن به وب سایت‌های دیگر آشنا میشویم. در مارک داون (Markdown) دو نوع لینک دادن وجود دارد، اما هر دو نوع به یک شکل دیده میشود.

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
