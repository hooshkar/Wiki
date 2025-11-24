---
title: Pull Request در گیت هاب (github)
author: محمد رضا کریمی
description:  pull request ها قلب همکاری در github هستند. هنگامی که شما یک pull request باز میکنید، در حقیقت شما تغییرات خود را پیشنهاد میکنید و درخواست میکنید تا کسی آن تغییرات را بررسی کند و در اصطلاح آن تغییرات را pull کند و آنها را با branch خود ادغام (merge) کند.
dateModified: 2025/11/24
datePublished: 2019/02/13
uid: It/SourceControl/Github/OpenPullRequest
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

Pull Request‌ها بخش کلیدی در فرآیند همکاری در **GitHub** هستند. این ابزار به شما اجازه می‌دهد تغییراتی که در یک **Branch** ایجاد کرده‌اید را پیشنهاد دهید، بازبینی کنید و سپس با Branch اصلی پروژه ادغام (Merge) کنید. 

## عملکرد Pull Request
- **پیشنهاد تغییرات**: با ایجاد Pull Request، تغییرات خود را برای بررسی دیگران ارسال می‌کنید.  
- **نمایش تفاوت‌ها**: GitHub تمام تغییرات بین Branch شما و Branch اصلی را به‌صورت بصری نمایش می‌دهد.  
- **ابزار بررسی**: با نمایش رنگ‌های سبز (اضافه شدن) و قرمز (حذف شدن)، می‌توانید تغییرات را دقیق‌تر بررسی کنید.  
- **مناسب برای یادگیری**: حتی می‌توانید برای پروژه‌های خودتان Pull Request ایجاد کنید تا با فرآیند کار آشنا شوید.

---

### **مراحل ایجاد Pull Request**

#### ۱. باز کردن Pull Request
1. وارد **Repository** خود شوید.  
2. در بالای صفحه، روی تب **Pull Requests** کلیک کنید.  
3. روی دکمه سبز رنگ **New Pull Request** کلیک کنید.

![باز کردن pull request](./Images/pr-tab.gif)

#### ۲. انتخاب Branch برای مقایسه
1. در بخش **Example Comparisons**، Branch‌ای که تغییرات در آن اعمال شده است (مثلاً `readme-edits`) را انتخاب کنید.  
2. این Branch با **Master Branch** (یا هر Branch اصلی دیگر) مقایسه خواهد شد.

![انتخاب branch](./Images/pick-branch.webp)

#### ۳. بررسی تغییرات
1. صفحه مقایسه تفاوت‌ها نمایش داده می‌شود.  
2. مطمئن شوید تغییراتی که در **readme-edits** ایجاد کرده‌اید، همان مواردی هستند که می‌خواهید ارسال کنید.  
3. تغییرات به‌صورت زیر نمایش داده می‌شود:  
   - **سبز**: نشان‌دهنده خطوط اضافه شده.  
   - **قرمز**: نشان‌دهنده خطوط حذف شده.

![مقایسه تفاوت ها](./Images/diff.webp)

#### ۴. ایجاد Pull Request
1. پس از بررسی، روی دکمه سبز رنگ **Create Pull Request** کلیک کنید.  
2. یک عنوان برای Pull Request بنویسید.  
3. توضیح مختصری درباره تغییراتی که اعمال کرده‌اید، اضافه کنید.  

![ارسال pull request](./Images/create-pr.webp)

#### ۵. ارسال Pull Request
1. پس از نوشتن پیام، روی دکمه **Create Pull Request** کلیک کنید.  
2. Pull Request شما اکنون ایجاد شده و آماده بررسی است.

![عنوان و توضیح pull request](./Images/pr-form.webp)

### نتیجه و نکات مهم
- **ایجاد گفتگو**: با Pull Request می‌توانید گفتگوهای مفید در مورد تغییرات داشته باشید.  
- **تمرین**: می‌توانید برای پروژه‌های شخصی نیز Pull Request باز کرده و تغییرات را خودتان ادغام کنید.  
- **پشتیبانی از همکاری تیمی**: ابزارهای GitHub نظیر Pull Request کار تیمی را ساده و شفاف‌تر می‌کند.

با این کار، فرآیند Pull Request کامل می‌شود و شما آماده مشارکت در پروژه‌های بزرگتر هستید.