# Tubey - بناء APK بدون Android Studio

1. أنشئ مستودع GitHub جديد وارفع كل محتويات هذا المجلد (مع مجلد .github).
2. افتح تبويب Actions وانتظر "Build APK" (حوالي 5-8 دقائق).
3. نزّل الملف من Artifacts: treasure-sort-apk، فك الضغط وثبّت app-debug.apk.

## الإعلانات (AdMob)
- حالياً تعمل بمعرّفات Google التجريبية (إعلانات وهمية آمنة).
- للنشر الحقيقي:
  1. أنشئ تطبيقاً في admob.google.com وأنشئ 3 وحدات إعلانية: Banner و Interstitial و Rewarded.
  2. في www/index.html عدّل الكائن ADS (ابحث عن ADS=): ضع المعرّفات الحقيقية و test:false.
  3. في GitHub: Settings > Secrets and variables > Actions > Variables، أضف ADMOB_APP_ID بقيمة معرّف التطبيق (ca-app-pub-xxx~yyy).
- لا تضغط على إعلاناتك الحقيقية أبداً (يسبب حظر الحساب).
- Google Play يطلب: سياسة خصوصية + نموذج Data safety يذكر استخدام AdMob.

## اسم الحزمة
appId مضبوط على iq.ekhtsar.tubey (لا يتغير بعد النشر). عند إنشاء التطبيق في AdMob وPlay Console استعمل نفس الاسم.
