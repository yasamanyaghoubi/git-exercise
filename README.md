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

