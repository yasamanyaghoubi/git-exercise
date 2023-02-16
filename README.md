## ۱ -گیت چیست و چه کاربردی دارد؟
گیت رایج ترین سیستم ورژن کنترل است. بدین صورت که تغییراتی که در فایل ها ایجاد میکنیم را ردیابی میکند بنابراین ما تاریخچه ای از کارهای قبلی مان را داریم و میتوانیم در صورت نیاز به آنها برگردیم.همچنین کار تیمی را آسانتر میکند و اجازه میدهد چند نفر بدون ایجاد تداخل روی یک پروژه مشترک کار کنند.

## ۲ -دستور init git چه کاری انجام میدهد؟
دستور git init یک ریپازیتوری جدید Git ایجاد می کند. می توان از آن برای تبدیل یک پروژه موجود و بدون نسخه به یک ریپازیتوری Git یا مقداردهی اولیه یک ریپازیتوری جدید و خالی استفاده کرد. اکثر دستورات دیگر Git خارج از یک ریپازیتوری اولیه در دسترس نیستند، بنابراین این دستور معمولا **اولین دستوری** است که در یک پروژه جدید اجرا می کنید.

## ۳ -دستور status git چه کاربردی دارد؟
دستور git status وضعیت دایرکتوری در حال کار بر روی آن و staging area را نمایش می دهد. این قابلیت به ما این امکان را می‌دهد که ببینیم کدام تغییرات انجام شده است، کدام یک انجام نشده است، و کدام فایل توسط Git ردیابی نمی‌شود. خروجی status هیچ اطلاعاتی در مورد سابقه پروژه commit  شده به شما نشان نمی دهد. برای دسترسی به این ویژگی باید از git log استفاده شود.

## ۴ -دستور add git چه کاری انجام میدهد؟
دستور git add تغییرات در دایرکتوری کاری را به staging area اضافه می کند. این دستور به Git می گوید که آیا کاربر می خواهد به روز رسانی های یک فایل خاص را در commit بعدی اضافه کند یا خیر. با این حال، git add واقعاً به هیچ وجه روی ریپازیتوری تأثیر نمی گذارد – (تا زمانی که git commit را اجرا نشود، تغییرات در واقع ثبت نمی شوند.)

## ۵ -دستور commit git چه کاری انجام میدهد؟
دستور git commit یک عکس فوری از تغییرات مرحله‌ای پروژه می‌گیرد. عکس های فوری از commit را می توان به عنوان نسخه های "ایمن" یک پروژه در نظر گرفت - Git هرگز آنها را تغییر نخواهد داد مگر اینکه شما صریحاً از آن درخواست کنید. قبل از اجرای git commit، دستور git add برای ارتقاء یا "مرحله" تغییرات در پروژه ای که در یک commit ذخیره می شود استفاده می شود. این دو دستور git commit و git add دو مورد از پرکاربردترین آنها هستند.

## ۶ -دستور log git چه کاربردی دارد؟
دستور git log تمام commit های تاریخچه ریپازیتوری را نمایش می دهد.

این دستور به طور پیش فرض این ویژگی ها را در هر commit نمایش می دهد:

1- الگوریتم هش ایمن (SHA) 
2- نویسنده
3- تاریخ
Message committing -4

## ۷ -دستور branch git چه کاری انجام میدهد؟
یک Branch نشان دهنده  توسعه و ارتقای یک خط مستقل است. شاخه ها می توانند به عنوان یک فرآیند ویرایش/stage/commit عمل کنند.می توان آنها را راهی برای درخواست یک دایرکتوری کاری جدید، staging area و تاریخچه پروژه در نظر گرفت. کامیت های جدید در تاریخچه برای شاخه فعلی ثبت می شود که منجر به یک فورک در تاریخچه پروژه می شود.

دستور git branch امکان ایجاد، فهرست، تغییر نام و حذف شاخه ها را می دهد.ولی به وسیله آن نمی توان بین شاخه‌ها جابجا شد یا یک تاریخچه فورک شده را دوباره کنار هم قرار داد. به همین دلیل، شاخه git تا حد زیادی با دستورات git checkout و git merge یکپارچه شده است.


## ۸ -دستور add remote git چه کاری انجام میدهد و چه کاربردی دارد؟
دستور Git remote add  یک دستور git است که به توسعه دهندگان این امکان را می دهد تا با ایجاد نسخه های تکراری روی یک ریپازیتوری مرکزی از راه دور کار کنند. دستور Remote Add به عنوان وسیله ای عمل می کند که از طریق آن همکاران یک پروژه می توانند به طور مستقل برای یک پروژه مشترک کامیت کنند. تابع Remote Add در git همچنین امکان فچ کردن تغییرات ایجاد شده از سرور راه دور به سرور لوکال را فراهم می کند. هنگام استفاده از git، باید یاد گرفت  که چگونه بین ریموت مرکزی به کنترل خود تغییر ایجاد کرد. به این ترتیب، می‌توان تمام به‌روزرسانی‌های status را حفظ کرد و از طریق روش‌های push و fetch git مشارکت داشت.


## ۹ -دستور push git چه کاری انجام میدهد؟
دستور git push برای آپلود محتوای ریپازیتوری محلی در یک مخزن راه دور استفاده می شود. Pushing نحوه انتقال کامیت ها از ریپازیتوری محلی خود به ریپازیتوری از راه دور است. این کار مانند همان فرایند فچینگ git است، اما در حالی که فچینگ مربوط به کامیت های محلی است ولی فرایند Pushing کامیت های ریموت را کنترل میکند. شاخه های راه دور با استفاده از دستور git remote پیکربندی می شوند.همچنین باید دقت داشت که  Pushingپتانسیل بازنویسی تغییرات را دارد پس هنگام پوش کردن باید احتیاط کرد.