# بناء APK من GitHub Actions (من الهاتف)

هذه الحزمة تحتوي على Workflow لبناء APK تجريبي تلقائياً. لا يحتاج الـWorkflow إلى كلمة مرور GitHub أو Personal Access Token أو أي Secret.

## الخطوات
1. سجّل الدخول إلى GitHub وأنشئ مستودعاً جديداً باسم `HR-Work-System-Android` واجعله Private.
2. من صفحة المستودع اختر Add file ثم Upload files.
3. ارفع **محتويات** مجلد `HR-Work-System-Android` بعد فك ضغط الحزمة (بما فيها المجلد المخفي `.github/workflows`). لا ترفع ملف ZIP وحده.
4. اضغط Commit changes.
5. افتح تبويب Actions، ثم اختر `Build Android APK`.
6. إذا لم يبدأ تلقائياً، اضغط Run workflow ثم Run workflow.
7. انتظر حتى تصبح العملية خضراء (Success)، وافتح نتيجة التشغيل.
8. من قسم Artifacts نزّل `HR-Work-System-debug-APK.zip`، ثم فك ضغطه لتحصل على `app-debug.apk`.
9. افتح APK على هاتف Android وثبّته بعد مراجعة مصدر الملف. قد يطلب Android السماح بالتثبيت من هذا المصدر.

## تنبيهات
- الناتج Debug APK للتجربة وليس إصدار متجر Google Play ولا APK إنتاجياً موقّعاً بمفتاح نشر.
- لا تشارك كلمات مرور GitHub أو رموز التحقق أو مفاتيح الاسترداد مع أي شخص.
- لا توجد في هذه النسخة خدمة خلفية أو مزامنة سحابية أو تسجيل دخول حقيقي؛ البيانات محلية على الجهاز والواجهة تحتوي بيانات تجريبية.
