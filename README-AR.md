# HR Work System — Android source project (v0.1.0)

هذه حزمة مشروع Android Studio لتغليف واجهة HR Work System الحالية داخل تطبيق Android مستقل يعمل محلياً دون اتصال بالإنترنت.

## ما الموجود
- واجهة HTML الحالية داخل `app/src/main/assets/index.html`.
- تطبيق Android أصلي بسيط باستخدام WebView لعرض الواجهة محلياً.
- حفظ بيانات النسخة التجريبية محلياً على الجهاز عبر WebView DOM Storage.
- لا توجد صلاحية إنترنت في Manifest، ولا يتصل التطبيق بخادم سحابي.

## بناء APK
1. افتح Android Studio على كمبيوتر.
2. اختر Open وافتح مجلد `HR-Work-System-Android`.
3. انتظر Gradle Sync، وثبّت Android SDK Platform 35 إذا طلبه Android Studio.
4. من القائمة Build اختر Build Bundle(s) / APK(s) ثم Build APK(s).
5. ملف APK التجريبي يظهر عادةً في `app/build/outputs/apk/debug/app-debug.apk`.

## حدود النسخة
- هذا مصدر مشروع Android وليس APK مبنياً أو موقعاً.
- لا يوجد تسجيل دخول حقيقي أو MFA أو حسابات Owner/Partner محمية بالخادم.
- الأسماء المعروضة داخل الواجهة ليست إثبات هوية أو صلاحيات.
- البيانات محلية على الجهاز وليست مشتركة بين مستخدمين أو شركات.
- توجد بيانات توضيحية داخل الواجهة؛ لا تستخدم بيانات موظفين حقيقية في هذه النسخة.
- الرواتب المعروضة ليست مسير رواتب قانونياً، والتكامل مع OpenAI/الدفع/الخدمات السحابية غير موصل.

## معرف التطبيق
`com.hrwork.system`
