---
title: قرار دادن عکس در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: در مارک داون (Markdown) مانند لینک دو نوع عکس وجود دارد، و هر دو نوع به یک شکل دیده میشود. تنها تفاوت لینک و عکس در این است که عکس با علامت تعجب آغاز میشود.
dateModified: 2018/05/16  
datePublished: 2018/05/16  
uid: It/Markdown/Images  
---
**راهنمای مطالب**

- [تصویر درون خطی (Inline Iamge)](#تصویر-درون-خطی-inline-iamge)
- [تصویر مرجع (Reference Image)](#تصویر-مرجع-reference-image)

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