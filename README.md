# Whispers of Betrayal — Android LAN Host

هذه النسخة تجعل الهاتف نفسه يستضيف خادم اللعبة عبر Wi‑Fi باستخدام WebSocket native داخل Android.

## طريقة البناء
1. افتح مجلد `android-host` في Android Studio.
2. انتظر مزامنة Gradle.
3. Build > Build APK(s).
4. ثبّت الـAPK على الهاتف المضيف وعلى هواتف الأصدقاء.
5. اربط كل الهواتف بنفس شبكة Wi‑Fi / Hotspot.
6. على الهاتف المضيف: افتح اللعبة واضغط **إنشاء غرفة**.
7. سيظهر عنوان مثل `ws://192.168.1.10:3000`.
8. على هواتف الأصدقاء: ضع هذا العنوان في **LAN Server** ثم اضغط Join.

## ملاحظة
اللعبة لا تحتاج إلى كمبيوتر أو Node.js عند تشغيل نسخة Android هذه. منطق اللعبة الأصلي موجود في `assets/www/host-engine.js` ويعمل داخل WebView، بينما WebSocket server المحلي يعمل داخل التطبيق نفسه.
