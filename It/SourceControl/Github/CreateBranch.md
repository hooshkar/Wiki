---
title: ایجاد و استفاده از Branch در گیت هاب
author: محمد رضا کریمی
description: هنگامی که شما یک branch از روی master branch ایجاد میکنید در واقع یک کپی از master branch در  لحظه میسازید.همچنین  وقتی که شما روی branch خود کار میکنید و افراد دیگر روی master branch تغییراتی را ایجاد میکنند، شما میتوانید آن تغییرات را نیز دریافت کنید.
dateModified: 2025/12/10
datePublished: 2019/02/13
uid: It/SourceControl/Github/CreateBranch
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

**Branching** یک روش بسیار مؤثر برای کار روی نسخه‌های مختلف یک **Repository** به صورت همزمان است. به طور پیش‌فرض، هر Repository یک **Branch** به نام **Master** دارد که به عنوان **Branch** اصلی در نظر گرفته می‌شود. **Branch**‌ها ابزارهایی برای آزمایش، ایجاد تغییرات و اطمینان از صحت آن تغییرات هستند، قبل از آنکه روی **Master Branch** اعمال شوند.

---

### **نحوه عملکرد Branch**
هنگامی که یک **Branch** جدید از **Master Branch** ایجاد می‌کنید، در واقع یک کپی از وضعیت فعلی **Master** در آن لحظه می‌سازید. در ادامه، می‌توانید تغییرات دلخواه خود را روی این **Branch** انجام دهید. اگر افراد دیگری روی **Master Branch** کار کنند، شما همچنان می‌توانید تغییرات جدید آن‌ها را دریافت و با **Branch** خود ادغام کنید.

---

### دیاگرام توضیحی
در یک دیاگرام ساده، می‌توان موارد زیر را مشاهده کرد:
1. **Master Branch** به‌عنوان شاخه اصلی.
2. یک **Branch** جدید با نام **Feature**.
3. مسیر **Feature Branch** از زمان ایجاد تا **Merge** شدن با **Master Branch**.

![ایجاد branch](./Images/branching.webp)

---

### **کاربرد Branch‌ها**
آیا تا به حال چندین نسخه از یک فایل را با نام‌های مختلف ذخیره کرده‌اید؟ مانند:
- `story.txt`
- `story-joe-edit.txt`
- `story-joe-edit-reviewed.txt`

**Branch‌ها** مشابه همین رویکرد عمل می‌کنند، اما در سطح Repository. 

در GitHub، توسعه‌دهندگان، نویسندگان و طراحان از **Branch** برای:
- نگهداری کد.
- رفع ایرادات.
- افزودن قابلیت‌های جدید.
- آزمایش ویژگی‌های خاص.

**Branch‌ها** تغییرات را از **Master Branch** جدا نگه می‌دارند. زمانی که تغییرات کامل و نهایی شد، می‌توان **Branch** را با **Master Branch** ادغام (Merge) کرد.

---

### **ایجاد یک Branch جدید در GitHub**
برای ایجاد یک **Branch** جدید مراحل زیر را دنبال کنید:

1. وارد **Repository** شوید که قبلاً ایجاد کرده‌اید.
2. در بالای لیست فایل‌ها، روی **Branch: master** کلیک کنید.
3. در کادری که باز می‌شود، نام **Branch** جدید (برای مثال: `readme-edits`) را وارد کنید.
4. روی دکمه **Create branch** (باکس آبی‌رنگ) کلیک کنید یا کلید **Enter** را بزنید.

![ایجاد branch جدید](./Images/readme-edits.gif)

اکنون شما دو **Branch** دارید: 
- **Master** 
- **Readme-edits**

این دو **Branch** در حال حاضر کاملاً شبیه به هم هستند. در مرحله بعد، شما می‌توانید تغییرات دلخواه خود را روی **Branch** جدید اعمال کنید. **Branching** در GitHub نه‌تنها ابزار قدرتمندی برای مدیریت نسخه‌ها است، بلکه همکاری مؤثرتر در پروژه‌های تیمی را نیز امکان‌پذیر می‌سازد.