---
title: انواع مختلف سورس کنترل و تفاوت آن ها
author: وحید برهانی
description: نرم‌افزارهای مدیریت کد (source control) به طور کلی به دو دسته توزیع شده (distributed) و متمرکز (centeralized) تقسیم می‌شوند که هر کدام از آن ها ویژگی های خاص خود را دارند.
dateModified: 2025/01/19
datePublished: 2019/09/20  
uid: It/SourceControl/TypeOfSC  
---

<blockquote style="background-color:#eeeefc; padding:0.5rem">
<details>
  <summary>آنچه در این مطلب خواهید خواند</summary>
  <ul>
    <li>نرم‌افزارهای مدیریت کد</li>
    <li>سورس کنترل مرکزی (Centralized Source Control)</li>
    <li>سورس کنترل توزیع‌شده (Distributed Source Control)</li>
    <li>تاریخچه مدیریت ورژن‌ها: از Subversion تا Git</li>
    <li>تفاوت Git و Subversion</li>
  </ul>
</details>
</blockquote>

داشتن ورژن‌های مختلف از فایل‌های یک پروژه نرم‌افزاری یا هر پروژه دیگری، همچون نگارش یک کتاب، به‌ویژه در پروژه‌های گروهی، از اهمیت ویژه‌ای برخوردار است. این کار نه تنها یک روش مطلوب برای حفظ تاریخچه تغییرات و پیشرفت‌ها به شمار می‌رود، بلکه در پروژه‌های گروهی و تیمی به امری ضروری تبدیل می‌شود. با استفاده از مدیریت مناسب ورژن‌ها، اعضای تیم می‌توانند به راحتی تغییرات خود را ثبت کرده و از مشکلات احتمالی در هنگام همگام‌سازی پروژه جلوگیری کنند.

## نرم‌افزارهای مدیریت کد

نرم‌افزارهای مدیریت کد از لحاظ نحوه نگهداری و مدیریت کد (source control) به دو دسته کلی تقسیم می‌شوند: **توزیع‌شده (distributed)** و **متمرکز (centralized)**. هر کدام از این روش‌ها ویژگی‌ها، مزایا و معایب خاص خود را دارند که به طور دقیق در ادامه بررسی خواهند شد.

### سورس کنترل مرکزی (Centralized Source Control)
در این روش، یک **سرور** مرکزی وجود دارد که تمامی تغییرات کد در آن ذخیره می‌شود. کاربران (برنامه‌نویسان) از **کلاینت‌ها** برای اعمال تغییرات یا دریافت تغییرات دیگران استفاده می‌کنند. به عبارت دیگر، در این سیستم، تمام اطلاعات و داده‌های مدیریتی و متادیتاها بر روی سرور نگهداری می‌شود و کلاینت‌ها تنها به یک نسخه مشخص از سورس کد دسترسی دارند.

**مزایا**:
- دسترسی به اطلاعات از یک نقطه متمرکز.
- ساده‌تر بودن مدیریت در مقیاس کوچک یا تیم‌های کوچک.

**معایب**:
- در صورتی که سرور از کار بیافتد یا دچار مشکل شود، کل فرآیند متوقف می‌شود.
- نیاز به اتصال آنلاین برای انجام تغییرات و دسترسی به کد.

### سورس کنترل توزیع‌شده (Distributed Source Control)
در این روش، سرور مرکزی وجود ندارد و هر فرد در تیم می‌تواند یک نسخه کامل از پروژه را در اختیار داشته باشد. تاریخچه کامل تغییرات هر فایل و متادیتاها به طور کامل در هر کلاینت ذخیره می‌شود. این امکان به کاربران اجازه می‌دهد که حتی بدون اتصال به اینترنت نیز تغییرات خود را اعمال کنند.

**مزایا**:
- امکان کار مستقل و بدون نیاز به اتصال آنلاین.
- هر کلاینت دارای یک نسخه کامل از پروژه و تاریخچه تغییرات است، بنابراین در صورت از کار افتادن سرور، کار ادامه پیدا می‌کند.
- امنیت بیشتر در حفظ تاریخچه و تغییرات.

**معایب**:
- نیاز به هماهنگی دقیق‌تر بین اعضای تیم در زمان همگام‌سازی تغییرات.

### تاریخچه مدیریت ورژن‌ها: از Subversion تا Git

پیش از توسعه روش‌های توزیع‌شده، بسیاری از تیم‌ها از سیستم‌هایی همچون **Subversion** (SVN) برای مدیریت کد استفاده می‌کردند. این سیستم‌ها تغییرات را نسبت به ورژن قبلی ذخیره می‌کردند، اما هنوز هم نیاز به سرور مرکزی داشتند و مشکلاتی مانند محدودیت‌های دسترسی آنلاین و عدم امکان ذخیره تمام نسخه‌ها وجود داشت. در این سیستم‌ها، کاربر نمی‌توانست به راحتی از همه نسخه‌ها استفاده کند و این فرآیند برای تیم‌ها محدودیت‌هایی به همراه داشت.

با معرفی **Git** در سال ۲۰۰۵ توسط **Linus Torvalds** (مخترع لینوکس)، این چالش‌ها حل شد. Git با استفاده از روش توزیع‌شده، دسترسی به تاریخچه کامل پروژه را به کاربران فراهم کرد و این امر باعث شد که Git تبدیل به یکی از محبوب‌ترین ابزارهای مدیریت کد در دنیای نرم‌افزار شود. اکنون بسیاری از پروژه‌ها به‌ویژه در پلتفرم‌هایی مانند **GitHub** و **GitLab** به کمک Git مدیریت می‌شوند.

![تفاوت git و subversion](./Images/centralized-vs-distributed.webp)

### تفاوت Git و Subversion

**Git** و **Subversion** (SVN) از نظر نحوه ذخیره‌سازی و همگام‌سازی تغییرات تفاوت‌های اساسی دارند:

- **Git** به صورت توزیع‌شده عمل می‌کند و هر کاربر نسخه کامل پروژه و تاریخچه تغییرات را در اختیار دارد.
- **Subversion** به صورت متمرکز است و تمامی تغییرات بر روی یک سرور مرکزی ذخیره می‌شوند.

این ویژگی‌های اساسی باعث شده‌اند که Git به ابزاری بسیار محبوب برای توسعه‌دهندگان تبدیل شود، به‌ویژه در پروژه‌های بزرگ و تیم‌های توزیع‌شده که نیاز به انعطاف‌پذیری بیشتری دارند.

### جمع‌بندی
در این مقاله به بررسی دو نوع مختلف از سیستم‌های مدیریت کد پرداخته شد: **سورس کنترل مرکزی** و **سورس کنترل توزیع‌شده**. همچنین تفاوت‌های کلیدی بین **Git** و **Subversion** (SVN) بررسی شد. در نهایت، با گسترش استفاده از ابزارهایی مانند Git و پلتفرم‌های محبوبی همچون **GitHub** و **GitLab**، تیم‌ها و توسعه‌دهندگان می‌توانند به راحتی تغییرات پروژه‌های نرم‌افزاری خود را مدیریت کنند.

اگر مایلید که اطلاعات بیشتری در خصوص source control ها داشته باشید با ما همراه شوید چرا که در ادامه به بررسی چند سرویس پرطرفدار و پرکاربرد نظیر github و tfs خواهیم پرداخت.