# محدودیت‌های فعلی / Known limitations

Reviewed 2026-10-27. This is a beta product, not the final stable release. / برنامه در مرحلهٔ بتاست و نسخهٔ پایدار نهایی منتشر نشده است.

| موضوع / Area | وضعیت / Status |
|---|---|
| پلتفرم / Platform | Windows x64 آزموده شده؛ پشتیبانی macOS/Linux ادعا نمی‌شود. / Windows x64 has been tested; macOS/Linux support is not claimed. |
| runtime و امضا / Runtime and signing | Electron 46 آلفا با انتخاب مالک پروژه استفاده می‌شود؛ بستهٔ فعلی بدون امضاست. / Electron 46 alpha is used by the project owner’s decision; current packages are unsigned. |
| زبان / Language | کنترل‌های اصلی، تنظیمات و راهنمای شروع دو زبانه‌اند؛ بعضی ابزارها، خطاها و یافته‌های تخصصی فارسی باقی‌اند. محتوای سایت ترجمه نمی‌شود. / Main controls, settings and the user guide are bilingual; some specialist tools, errors and findings remain in Persian. Site content is never translated. |
| Licence | فعال‌سازی لازم نیست؛ دو فرمان Licence غیرفعال‌اند. / No activation is required; both Licence commands are disabled. |
| Google | اتصال پیش‌فرض عمومی در این بتا ارائه نمی‌شود؛ بستهٔ CI فایل OAuth توسعه‌دهنده را ندارد. واردکردن Desktop OAuth متعلق به خود کاربر در تنظیمات پیشرفته ممکن است؛ تابع مجوزها و الزامات Google است. / This beta does not ship the developer's default OAuth client. Advanced users can import their own Desktop OAuth configuration, subject to Google's permissions and publishing requirements. |
| GA4 و PageSpeed | دادهٔ غیرصفر GA4 با حساب آزمایش در دسترس نبود؛ PageSpeed بدون کلید محدودیت سهمیه داشت. این وضعیت به معنی نبود قابلیت یا نبود مشکل سایت نیست. / Nonzero GA4 data was unavailable for the test account; keyless PageSpeed hit a quota limit. These are not clean-site results. |
| AI | متن Gemini/Ollama مسیر مستقل دارد؛ خروجی تصویر/صوت AI غیرفعال است. / Text analysis has Gemini/Ollama paths; AI image/audio exports are disabled. |
| Semantically Similar | خروجی آن در Bulk Export غیرفعال است. Content Cluster Diagram با تولید دستی Embeddings محلی، قابلیت جداگانه‌ای است. / Its Bulk Export entry is disabled. Content Cluster Diagram separately uses manually generated local embeddings. |
| Ollama | سرور و مدل مناسب باید آماده باشند؛ دانلود یا اجرای خودکار مدل وجود ندارد. / Requires a running server and installed model; the app does not automatically download or start models. |
| داده و پوشش / Coverage | سقف URL، قواعد، منابع مسدود و capture غیرفعال پوشش را محدود می‌کنند. / URL limits, configuration, blocked resources and disabled capture limit coverage. |
| حافظه / RAM | تغییر ذخیره‌نشده پس از خروج ناگهانی می‌تواند از بین برود؛ گزارش موقت جای ذخیرهٔ جلسه نیست. / An unexpected exit can lose unsaved RAM changes; temporary report files are not session saves. |
| رندر / Rendering | پایان snapshot تضمین تکمیل تعامل‌ها یا lazy-load نیست؛ نمایشگر تشخیصی اجرای زندهٔ همهٔ رفتارهای سایت را بازسازی نمی‌کند. / Snapshots do not guarantee completed interactions or lazy loading, and the diagnostic viewer does not reproduce every live site behaviour. |

حدود سنجش کارایی، حفظ داده و پذیرش Windows در مستندات فنی پروژه ثبت شده‌اند؛ سقف تنظیمات، ظرفیت تضمین‌شده روی هر رایانه نیست. / Performance and durability evidence has a defined scope; configuration bounds are not guaranteed capacity on every machine.
