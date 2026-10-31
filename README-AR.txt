MISHRADAR — نقل الموقع إلى الرابط الجديد (2026-10-31)
======================================================
الرابط الجديد المستهدف: https://ozaapex.github.io/mishradar/
المستودع الجديد: https://github.com/OZAapex/mishradar

تحتوي الحزمة على ملفات الموقع ذات العلامة الجديدة والروابط المصححة،
وقواعد عرض الوظائف، وملف GitHub Actions، وإصلاح الفواتير السابق.

خطوات العمل بدون حذف أو تغيير المشروع القديم:
1) فك ضغط الحزمة على الكمبيوتر.
2) من المستودع القديم https://github.com/OZAapex/mishrali اضغط Code > Download ZIP.
3) افتح الملف القديم واستخرج منه config.js الحالي كما هو، وانقله إلى مجلد
   Mishradar-Migration-Ready بجانب index.html. لا تنشر مفتاح secret/service_role.
4) إذا عندك ملف Google للتحقق باسم google*.html، انسخه أيضًا إلى الجذر
   ليستمر تحقق Search Console عند الحاجة.
5) افتح المستودع الجديد https://github.com/OZAapex/mishradar، ثم Add file > Upload files.
   اسحب محتويات مجلد Mishradar-Migration-Ready بكاملها (بما فيها .github وscripts)
   إلى صفحة الرفع. لا ترفع ZIP مضغوطًا.
6) Commit changes.
7) من المستودع الجديد افتح Settings > Pages > Build and deployment > Source
   واختَر GitHub Actions.
8) انتقل إلى Actions وشغّل Publish Mishradar website and public job pages.
9) بعد Success تأكد أن https://ozaapex.github.io/mishradar/ يعمل، وكذلك
   /pricing.html و/jobs/ و/sitemap.xml.
10) اختبر تسجيل دخول المدير والوظائف وطريقة التقديم وتسجيل الشركات والرسوم.
11) فقط بعد نجاح الاختبارات: Search Console أضف عنوان /mishradar/، أرسل
    https://ozaapex.github.io/mishradar/sitemap.xml واطلب فهرسة الجديد.
12) اترك المستودع والموقع القديمين كما هما في الوقت الحالي. في خطوة منفصلة
    سنختار كيفية إعادة توجيه الزائرين والروابط القديمة بأمان.

لا تغيّر Supabase ولا تشغل SQL جديد ولا تحذف المستودع القديم.
لا تحذف أي شركة أو وظيفة أو رسوم من قاعدة البيانات.
النقل إلى المسار الجديد يتطلب تحديث عناوين صفحات الموقع وملف sitemap.
ملاحظة: هذا البناء من ملفات آخر حزمة متوفرة في المحادثة، ولم يُجلب مباشرةً
من المستودع الحي. إذا عدّلت ملفات الموقع بعد آخر تحديث، راجع الفروقات قبل الرفع.
ملاحظة: مجرد ظهور موقعين على نفس قاعدة البيانات يعني أي إضافة/تعديل وظائف
تظهر بالموقعين إلى حين فصل أو إيقاف القديم؛ لا تستخدمه لتجارب حذف.
