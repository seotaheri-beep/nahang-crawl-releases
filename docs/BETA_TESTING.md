# آزمایش بتا / Beta testing — 1.0.0-beta.1

این نسخه برای بازخورد پیش از انتشار پایدار است. برنامه یک نسخهٔ واحد و بدون نیاز به فعال‌سازی دارد. بستهٔ Windows x64 بدون امضای دیجیتال است و Electron همراه آن هنوز آلفاست. محدودیت‌های [Google، زبان و سرویس‌ها](KNOWN_LIMITATIONS.md) را بخوانید.

This is a preview for feedback before a stable release. There is one edition and no activation. Windows x64 packages are unsigned and the bundled Electron runtime is alpha. Read the [known limitations](KNOWN_LIMITATIONS.md), especially Google access and partial specialist translations.

## پیش از شروع / Before starting

- بسته و SHA-256 را از همان [انتشار رسمی](https://github.com/seotaheri-beep/nahang-crawl-releases/releases) بگیرید. / Get the package and SHA-256 from the same official release.
- پیش از ارتقا، خزش فعال را تمام/متوقف و داده‌های مهم را با فایل خزش یا پشتیبان ذخیره کنید. برای ZIP همهٔ فایل‌ها را در پوشه‌ای تازه استخراج کنید. / Finish or stop active work and save important data before upgrading. Extract the entire ZIP into a new folder.
- فقط سایت دارای مجوز را آزمایش کنید؛ برای شروع سقف ۵۰۰ URL و سرعت پیش‌فرض کافی است. / Use an authorised site; start with 500 URLs and the default speed.
- مدل Ollama، API پولی، حساب Google و ارسال ایمیل برای این فهرست لازم نیست. / No model, paid API, Google account or email transmission is required.

## سناریو / Checklist

1. نصب‌کننده یا نسخهٔ ZIP را اجرا کنید؛ نسخهٔ پایین پنجره باید `1.0.0-beta.1` باشد. / Launch Setup or the portable app; confirm the footer version.
2. F1 بزنید، راهنمای شروع را بخوانید و یک خزش کوچک انجام دهید. / Open F1, read Quick Start and run a small crawl.
3. نتیجه‌ای را با ماوس و سپس صفحه‌کلید انتخاب کنید؛ عنوان، کد پاسخ، لینک‌های ورودی و خروجی را بررسی کنید. / Select a row with mouse and keyboard; inspect its title, response and links.
4. جست‌وجو/فیلتر و خروجی CSV را بررسی کنید؛ عنوان فارسی سایت باید حفظ شود. / Search/filter and export CSV; Persian site content should be preserved.
5. فایل خزش را ذخیره کنید؛ خزش تازه بسازید و فایل را دوباره باز کنید. داده‌های خزش ذخیره‌شده باید برگردند. / Save a Crawl File, open a New view and import the file; saved results should return.
6. برنامه را ببندید و باز کنید؛ تاریخچه، تنظیمات و خزش ذخیره‌شده را بررسی کنید. / Restart and inspect history, settings and saved data.
7. رابط فارسی/انگلیسی و روشن/تیره را امتحان کنید. متن سایت نباید ترجمه شود. / Try Persian/English and light/dark; site content should not be translated.
8. از Help → Check for Updates استفاده کنید؛ پس از انتشار این بتا، نسخهٔ بتای فعلی نباید همان نسخه را به‌عنوان آپدیت تازه پیشنهاد دهد. / Check for Updates; this beta should not offer itself as a newer update.

در صورت تمایل، یک آزمون جدا با JavaScript و سقف کوچک اجرا کنید؛ حالت رندر و محدودیت‌های مشاهده‌شده را در گزارش بنویسید. / Optionally repeat a small crawl with JavaScript rendering and record the mode and observed limits.

## ثبت نتیجه / Record the result

نسخهٔ Windows، معماری، نصب یا ZIP، RAM تقریبی، حالت ذخیره، رندر، اندازهٔ آزمون و نتیجهٔ هر مرحله را ثبت کنید. شکست را با مراحل بازتولید و نتیجهٔ مورد انتظار/واقعی در [Issues](https://github.com/seotaheri-beep/nahang-crawl-releases/issues) گزارش کنید. قالب و احتیاط دربارهٔ اطلاعات خصوصی در [پشتیبانی](SUPPORT.md) است. ارسال عمومی لاگ، کوکی، کلید، URL خصوصی یا فایل کامل خزش لازم نیست.

Record Windows version, architecture, Setup/ZIP, approximate RAM, storage/rendering modes, test size and each step's outcome. Report failures with reproduction steps and expected/actual behaviour in Issues. Use the [support template](SUPPORT.md); do not post credentials, cookies, private URLs or complete private crawls.

تا زمان دریافت گزارش واقعی، بازخورد کاربران بیرونی «دریافت نشده» است؛ نتیجهٔ خودکار یا آزمایش توسعه‌دهنده، بازخورد کاربر بیرونی محسوب نمی‌شود. / External feedback is pending until real reports arrive; automated/developer tests are not independent user feedback.
