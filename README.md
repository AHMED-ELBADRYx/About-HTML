# شرح HTML بالعربية

هذا دليل مبسط وشامل لأهم أوامر HTML الأساسية مع الأمثلة.

---

## فهرس المحتويات

1. [مقدمة عن HTML](#مقدمة-عن-html)
2. [الهيكل الأساسي للصفحة](#الهيكل-الأساسي-للصفحة)
3. [العناوين والفقرات](#العناوين-والفقرات)
4. [تنسيق النصوص](#تنسيق-النصوص)
5. [الروابط](#الروابط)
6. [الصور](#الصور)
7. [خصائص اتجاه النص](#خصائص-اتجاه-النص)

---

## مقدمة عن HTML

هذا الدليل يشرح العناصر الأساسية في HTML مع أمثلة عملية لكتابتها بشكل صحيح.

---

## الهيكل الأساسي للصفحة

```sh
<!DOCTYPE html>
<html lang="ar">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>عنوان الصفحة</title>
    <link rel="stylesheet" href="style.css">
    <style>
      /* CSS هنا */
    </style>
  </head>
  <body>
    <!-- المحتوى -->
  </body>
</html>
```

## لتحديد نوع المستند

 ```sh
<!DOCTYPE html>
```

## كل الصفحة بعدها حتى النهاية يتم كتايتها بين

```sh
<html>
</html>
```

## داخلها يوجد قسمين أساسيين

### قسم لمعلومات الموقع يكون بين

```sh
<head>
</head>
```

### قسم يظهر للمستخدم يكون بين

```sh
<body>
</body>
```

---

## داخل رأس الموقع

---

## لدعم أغلب اللغات ومنها العربية

```sh
<meta charset="utf-8">
```

## لتحديد لغة الموقع نفسه فنكتبها في html

```sh
<html lang="ar">
```

## لكتابة اسم الموقع تكون بين

```sh
<title>
</title>
```

## لتحديد وصف الموقع

```sh
<meta name="description" content="ما سيظهر للمستخدم في وصف الموقع">
```

## لظهور الموقع عند بحث معين

```sh
<meta name="keywords" content="html , css , php">
```

## لتحديد صاحب الموقع

```sh
<meta name="author" content="My name">
```

## لجعل الموقع متجاوبًا

```sh
<meta name="viewport">
```

## لتحديث الموقع كل مدة معينة مثلا 3 ثواني

```sh
<meta http-equive="refresh" content="3">
```

### مثلا إن انتقلنا لموقع جوجل خلال 4 ثواني تكون

```sh
<meta http-equive="refresh" content="5" url=https://www.google.com/>
```

## للبحث عن كل أنواع الميتا اضغط [هنا](https://www.w3schools.com/tags/tag_meta.asp)

## لربط CSS خارجي

```sh
<link rel="stylesheet" href="css/style.css">
```

- rel="stylesheet" : هو نوع علاقة الربط بملفات css
- href="css/style.css" : هو موقع الملف

## لكتابة CSS داخلي

```sh
<style>
</style>
```

## لكتابة Java script داخلي

```sh
<script>
</script>
```

---

## داخل جسم الموقع (body)

---

## الأوسمة تنقسم لقسمين

- block: تنشئ سطرا جديدا (خاصة بالعناوين والفقرات)
- inline: تكون في نفس السطر (خاصة بتنسيق النصوص بدلا من css)

---

## العناوين والفقرات

- العناوين:

```sh
<h1>الأكبر</h1>
<h6>الأصغر</h6>
```

- الفقرة:

```sh
<p>نص الفقرة هنا.</p>
```

- سطر جديد:

```sh
<br>
```

- خط فاصل:

```sh
<hr>
```

- لمراعاة المسافات البادئة والأسطر الجديدة لمجموعة نصوص (مثل الأكواد)

```sh
<code>
<pre>
if True:
  print("Hello!")
</pre>
</code>
```

---

## تنسيق النصوص

- غامق:

```sh
<b>غامق</b>
<strong>هام</strong>
```

- مائل:

```sh
<i>مائل</i>
<em>مؤكد</em>
```

- تحته خط:

```sh
<u>مسطر</u>
<ins>مضاف</ins>
```

- مشطوب:

```sh
<s>محذوف</s>
<del>ملغى</del>
```

- مميز بالأصفر:

```sh
<mark>مميز</mark>
```

- نص منخفض ومرتفع:

```sh
X<sub>2</sub>
10<sup>3</sup>
```

- صغير:

```sh
<small>صغير</small>
```

---

## الروابط

- رابط أساسي:

```sh
<a href="https://example.com">رابط</a>
```

`target="_self"`: نفس النافذة (افتراضي)

- فتح في نافذة جديدة:

```sh
<a href="https://example.com" target="_blank">رابط جديد</a>
```

`https://`: يعني أنه رابط من موع خارجي

- رابط تنزيل:

```sh
<a href="file.pdf" download="اسم الملف بعد التحميل">تحميل</a>
```

`download`: قيمتها اختيارية

- ليس شرطا أن يكون الرابط في النص فيمكن استخدام أي وسم مثل وسم الصور مثلا:

```sh
<a href="https://example.com">
    <img src="image.jpg"
</a>
```

### الانتقال

- يمكن أيضا للرابط أن ينقل لقسم آخر بنفس الصفحة من خلال كتابة اسم الوسم الذي به القسم وإن كان الوسم متكرر بقسم آخر فنقوم بإعطائه معرف خاص يميزه من خلال id وكتابته من خلال # مثلا:

```sh
<h1 id="x">مرحبًا</h1>
<h1>أهلًا</h1>
<a href="#x">انتقل إلى مرحبا</a>
```

- يمكن أيضا الانتقال لإيميل للتواصل:

```sh
<a href="mailto:example@gmail.com">تواصل عبر الإيميل</a>
```

`mailto`: معرف الإيميل

- التواصل عبر الهاتف:

```sh
<a href="tel:0123456789">تواصل عبر الهاتف</a>
```

`tel`: معرف الهاتف

- الانتقال لكود جافا سكريبت:

```sh
<a href="javascript:alert('Hello!');">كود جافا سكريبت</a>
```

`javascript`: معرف جافا سكريبت

---

## الصور

- صورة أساسية:

```sh
<img src="image.jpg" alt="وصف" width="300" height="200">
```

- خصائص إضافية:

```sh
<img src="img.jpg" alt="..." title="شرح" loading="lazy">
```

- src: هو مصدر الصورة
  
### يجب ان نكتب الصورة بمسارها الصحيح فنكتب اسمها فقط لو كانت داخل مجلد المشروع مباشرة أو لو كانت داخل المجلد فنكتبها كما هي داخل المجلد مثل `folder\img.jpg` أو لو كانت في مسار آخر أصلا فنكتب المسار كامل هكذا مثلا `D:....\Images` أو لو كانت الصورة من موقع خارجي مثل جوجل فنكتب رابطها الخاص

- alt: هو ما يصف الصورة في حالة عدم عرضها

- title: هو النص الظاهر على صورة حينما نضع المؤشر عليها
- loading="lazy" : تحميل الصورة فقط أثناء القرب منها

---

## خصائص اتجاه النص

- من اليمين إلى اليسار:

```sh
<body dir="rtl">
```

- من اليسار إلى اليمين:

```sh
<body dir="ltr">
```

---

## الجداول

```sh
<table border="1" width="100%" bgcolor="#f2f2f2" align="center">
 <caption>وصف</caption>
  <thead>
    <tr>
      <th>عنوان 1</th>
      <th colspan="2">عنوان 2 و3 مدمجين</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">صف مدمج 1 و2</td>
      <td>خلية 2</td>
      <td>خلية 3</td>
    </tr>
    <tr>
      <td>خلية 2-2</td>
      <td>خلية 3-2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="3">خاتمة الجدول</td>
    </tr>
  </tfoot>
</table>
```

- caption: وصف الجدول أو موضوعه
- thead: رأس الجدول (العناوين)
- tbody: جسم الجدول (العناصر)
- tfoot: زيل الجدول (النتائج)

### تبقى مواقعها ثابتة وأن تغير ترتيبها في الكود

- tr: صف
- td: عمود
- th: عنوان (سميك)
- border لتحديد سمك الحدود.
- colspan لدمج الأعمدة (يعني لو صف به عدد أعمدة أقل يتم دمجها بالأعمدة الناقصة)
- rowspan لدمج الصفوف (العكس)
- bgcolor: تحديد اللون (يمكن تحديده على أي وسم)

---

## القوائم

### قائمة مرقمة

```sh
<ol type="A">
  <li>الخيار الأول</li>
  <li>الخيار الثاني</li>
</ol>
```

- النوع: 1، A، a، I، i
- reversed: عكس الترتيب
- start="7": بداية العد من 7

---

### قائمة غير مرقمة

```sh
<ul type="circle">
  <li>عنصر 1</li>
  <li>عنصر 2</li>
</ul>
```

- الأنواع: disc (افتراضي)، circle، square

---

### قائمة وصفية

```sh
<dl>
  <dt>المصطلح</dt>
  <dd>الشرح المفصل</dd>
</dl>
```

---

## تفاصيل قابلة للطي

```sh
<details>
  <summary>عن الموقع</summary>
  <p>نص توضيحي هنا.</p>
  <img src="pic.jpg" alt="صورة">
  <br>
  <img src="pic2.jpg" alt="صورة ثانية">
</details>
```

- الصور ستتوالى تحت بعضها باستخدام `<br>`.

---

## الحاويات

### حاوية عامة

- عنصر block، يأخذ عرض السطر بالكامل.

```sh
<div>
  المحتوى هنا
</div>
```

#### يوجد حاويات مختلفة على حسب نوع المحتوى

- `<header>`: الجزء العلوي
- `<nav>`: شريط التنقل
- `<main>`: المحتوى الرئسيسي
- `<section>`: القسم
- `<article>`: المقالة
- `<aside>`: الشريط الجانبي
- `<footer>`: الجزء السفلي

---

### عنصر داخل السطر

- عنصر inline، يبقى في السطر نفسه.

```sh
<span>نص صغير</span>
```

---

## إضافة فيديو وصوت

### فيديو

```sh
<video src="video.mp4" width="400" height="300" controls poster="cover.jpg">
  المتصفح لا يدعم الفيديو
</video>
```

#### وحدة الحجم الافتراضية هي `px` يمكن وضع وحدات أخرى مثل `%` ليكون حجمها مقارن بحجم المتصفح

- controls: لإظهار أزرار التشغيل
- poster: صورة مصغرة قبل التشغيل
- muted: كتم الصوت افتراضيًا
- autoplay: تشغيل تلقائي (فقط في حالة `muted` لتجنب الإزعاج)
- loop: تكرار تلقائي
- preload:
  - auto: تحميل تلقائي
  - none: لا يتم التحميل إلا عند التشغيل
  - metadata: تحميل معلومات الملف فقط

#### بعض المتصفحات لا تدعم امتدادات معينة لذا نحتاج لعرض الفيديو بأكثر من امتداد من خلال `source`

```sh
<audio controls>
    <source src="video.mp4" type="audio/mp4">
    <source src="video.ogg" type="audio/oog">
    <source src="video.webm" type="audio/webm">
    <track src="en.vtt" kind="subtitles" label="English">
</audio>
```

- source:
  - type: يحدد نوع الصورة
- track: لإضافة ملفات الترجمة
  - src: مكان ملف الترجمة
  - kind: نوع الملف
  - label: اسمها الظاهر أثناء اختيارها
  - default: ترجمة تلقائية

---

### صوت

```sh
<audio src="sound.mp3" controls muted preload="auto">
  المتصفح لا يدعم الصوت (تظهر الرسالة في حالة أن الصوت غير مدعوم)
</audio>
```

- controls: لإظهار أزرار التشغيل
- muted: كتم الصوت افتراضيًا
- autoplay: تشغيل تلقائي (توقف دعمها لآزعاجها)
- loop: تكرار تلقائي
- preload:
  - auto: تحميل تلقائي
  - none: لا يتم التحميل إلا عند التشغيل
  - metadata: تحميل معلومات الملف فقط

#### بعض المتصفحات لا تدعم امتدادات معينة لذا نحتاج لعرض الصوت بأكثر من امتداد من خلال `source`

```sh
<audio controls>
    <source src="music.mp3" type="audio/mpeg">
    <source src="music.ogg" type="audio/oog">
    <source src="music.wav" type="audio/wav">
</audio>
```

- source:
  - type: يحدد نوع الصورة

#### نفس الأمر ينطبق مع الفيديو أيضا

---

## روابط وصفحات خارجية

```sh
<a href="https://example.com" target="_blank">افتح الموقع</a>
```

- target="_blank": لفتح الرابط في نافذة جديدة
- target="_self": (افتراضي) نفس النافذة

---

### روابط داخلية

```sh
<a href="about.html">حول الموقع</a>
```

- الروابط النسبية تُكتب حسب موقع الملف الحالي.

---

## الصور وصور GIF

```sh
<img src="image.gif" alt="صورة متحركة" width="300" height="200">
```

- يمكن استخدام GIF تمامًا كالصورة.

---

## التضمين داخل إطار

- يستخدم لتضمين مواقع، فيديوهات، PDF... إلخ
- هناك مواقع لا تسمح بعمل تضمين لها
- يوجد ثلاثة أوسمة لها
  - iframe
  - object
  - embed

---

### iframe

```sh
<iframe frameborder="0" src="https://example.com" width="500" height="300"></iframe>
```

- غير محافظ على أبعاد الصور
- يعمل على أي متصفح على أي نظام
- frameborder: يتحكم في وجود الإطار (0: غير موجود، 1: موجود)
- scrolling="no": يزيل مؤشر التحرك

---

#### تضمين فيديو يوتيوب

- من اليوتيوب: كليك يمين على الفيديو → "نسخ رمز التضمين"
- النتيجة تكون مثل:

```sh
<iframe width="560" height="315"
src="https://www.youtube.com/embed/ID"
title="YouTube video" frameborder="0"
allowfullscreen></iframe>
```

- allowfullscreen: السماح بملأ الشاشة

---

### object

```sh
<object data="https://example.com" width="500" height="300"></object>
```

- date: مثل `src`
- بدون إطالر

---

### embed

```sh
<embed src="https://example.com" width="500" height="300">
```

- وسم غير مغلق
- بدون إطالر

---

## النماذج (Forms)

### زر

```sh
<input type="button" value="اضغط هنا">
```

أو:

```sh
<button type="button">اضغط هنا</button>
```

---

### نموذج تسجيل

```sh
<form>
  <input type="text" placeholder="اسم المستخدم">
  <br>
  <input type="password" placeholder="كلمة السر">
  <br>
  <input type="email" placeholder="البريد الإلكتروني">
  <br>
  <input type="number" placeholder="السن">
  <br>
  <input type="tel" placeholder="رقم الهاتف">
  <br>
  <input type="submit" value="تسجيل">
</form>
```

- input: إدخال البيانات
  - type: نوع الإدخال
    - text: مربع نصي
    - number: مربع رقمي
    - password: بيانات سرية مخفية
    - email: يجب أن يكون مصحوبا بـ @
    - tel: رقم الهاتف
    - reset: زر مسح البيانات
    - submit: زر إرسال البيانات
    - button: زر عادي بحاجة إلى `value`
    - radio: تحديد خيار واحد من مجموعة خبارات
    - checkbox: تحديد أكثر من خيار
    - color: تحديد لون الحقل
    - file: تحديد ملف من الجهاز
    - range: تحديد مقدار القيمة
    - search: البحث
    - url: إضافة رابط
    - hidden: إخفاء الحقل (مثل حقل الـ id الذي سيتم إرساله)
    - datetime-local: إضافة التواريخ والأوقات
    - date: إضافة التواريخ (يوم، شهر، سنة)
    - month: إضافة الشهور والسنين
    - week: إضافة أيام الأسبوع
    - time: إضافة الأوقات (الساعات والدقائق والأزمنة (صباحًا، مساءً))
  - checked: لتحديد القيمة مبدئيًا مثل في الـ radio (يمكن تغييرها)
  - disabled: زر غير قابل للتحديد
  - value: قيمة نضعها في الحقل مثل زر الـ submit لتغيير اسمه أو اسم المستخدم القديم لو أراد تعديله وهي وهي القيمة يتم إرسالها عبر submit
  - min: أقل قيمة يمكن تحديدها
  - max: أكبر قيمة يمكن تحديدها
  - step: مقدار الخطوات (1 افتراضيا)
  - value, min, max, step: يمكن استخدامها مع range, number
  - id: المعرف المميز للحقل
  - placeholder: نص مساعد داخل الحقل يختفي بمجرد الكتابة عليه
  - autofocus: تفعيل الحقل
  - readonly: غير قابل لإدخال البيانات لكنه يرسل بيانات الـ `value` إن وجدت
  - disabled: غير قادر على تفعيل الحقل لإدخال البيانات ولا يرسل بيانات الـ `value` مثل الـ `id` مثلا
  - required: البيانات مطلوبة للإرسال
  - input type: يمكن اختصارها إلى `input:`

---

### أسئلة متعددة الاختيارات

```sh
<!-- عناصر النموذج -->
<form method="get" action="file.php">

  <!-- إطار خارجي -->
  <fieldset>
  <legend>عنوان</legend>

    <!-- نموذج السؤال -->
    <p>ما هو لونك المفضل؟</p>
    <label for="id value">
        <input type="radio" name="color" value="red" checked>
        أحمر
    </label>
    <br>
    <label>
        <input type="radio" name="color" value="blue">
        أزرق
    </label>
    <br>

    <!-- نموذج التحديد -->
    <p>ما هو جنسك؟</p>
    <label>
      <select name="gender">
        <optgroup label="الجنس">

          <option value="male" selected>
          ذكر
          </option>

          <option value="female">
          أنثى
          </option>

        </optgroup>


        <optgroup label="النوع">

          <option value="other">
          آخر
          </option>

          <option value="prefer_not_to_say">
          أفضل عدم القول
          </option>

        </optgroup>
      </select>
    </label>
    <br>

    <!-- نموذج البحث مع التحديد -->
    <input list="colors" name="color_input" placeholder="أدخل لونك المفضل">
    <datalist id="colors">
      <option value="أحمر">
      <option value="أزرق">
      <option value="أخضر">
      <option value="أصفر">
    </datalist>
    <input type="submit" value="إرسال">
  </fieldset>
</form>
```

#### عناصر النموذج

- method: التحكم في غظهار البيانات في ششريط البروتوكول
  - get: إظهار البيانات مثل بيانات البحث (افتراضيا)
  - post: حماية البيانات وإخفائها مثل بيانات كلمة السر
- action: الصفحة التي تُرسل إليها البيامات من خلال زر الإرسال (القيمة الإفتراضية هي الصفحة نفسها)
- novalidate: يسمح بالإرسال دون إدخال أي قيمة
- target: نافذة الإلرسال
  - "_self": نفسها (افتراضيا)
  - "_blank": نافذة جديدة

#### إطار خارجي

- fieldset: إحاطة كل الحقول بحقل خارجي
- legend: عنوان الإطار الخارجي

#### نموذج السؤال

- label: وصف المدخل
  - for: قيمته هي قيمة الـ id في الـ input الذي يفعل الحقل الخاص به
- name: اسم حقل السيرفر الذي سيتم إرسال البيانات أو الـ `value` إليه وإعطاؤه نفس القيمة في أكثر من `input` يعني أنه يجب تحديد حقل واحد منهم فقط (عند استخدامها مع `radio`)

#### نموذج التحديد

- select: إنشاء قائمة منسدلة (يسمح بالبحث بدون إظهار المحرك)
- optgroup: مجموعة أقسام خيارات
- label: وصف القسم
- option: إنشاء خيارات للقائمة
- multiple: تحديد عدة خبارات (`CTRL+CLICK`)
- selected: تحديد مبدئي (يمكن تغييره)

#### نموذج البحث مع التحديد

- input list: يظهر محرك البحث عكس `select` قيمته هي قيمة الـ id (مثل: `label for`)
- datalist: قائمة الخيارات
- option: هنا وسم غير مغلق لأن قيمة الـ value هي نفسها القيمة الظاهرة

---

### حقل نص طويل

```sh
<textarea rows="5" cols="30" minlength="4" maxlength="10">اكتب رسالتك هنا...</textarea>
```

- rows: عدد الصفوف
- cols: عدد الأعمدة (افتراضيا: 20)
- minlength: أقل عدد حروف يمكن إدخالها
- maxlength: أكثر عدد حروف يمكن إدخالها
- يمكن استخدامهما مع `type text`

---

### عناصر تنسيق

```sh
<br>  <!-- سطر جديد -->
<hr>  <!-- خط فاصل -->
```

---

## أنواع العناصر في HTML

### Block مقابل Inline

#### عناصر Block

- تأخذ كامل عرض السطر
- تبدأ من سطر جديد
- يمكن تغيير العرض والطول

أمثلة:

```sh
<div></div>
<p></p>
<h1></h1>
<ul></ul>
<li></li>
<table></table>
```

---

#### عناصر Inline

- تظهر في نفس سطر النص
- لا يمكنها أخذ عرض/طول بشكل افتراضي
- تُستعمل داخل عناصر أخرى

أمثلة:

```sh
<span></span>
<a href=""></a>
<strong></strong>
<em></em>
<img>
```

---

### الفرق في التنسيق

| الخاصية       | Block         | Inline         |
| -------------- | ------------- | --------------- |
| العرض والطول    | مسموح         | لا يعمل افتراضيًا |
| الخلفية         | يغطي السطر كله | يغطي النص فقط  |
| Margin/Padding | جميع الجهات    | فقط Left/Right  |

---

## خصائص العرض (Display)

- display: block; — يحول العنصر إلى Block
- display: inline; — يحوله إلى Inline
- display: inline-block; — مثل inline لكن يسمح بالعرض والطول
- display: none; — يخفي العنصر ويزيله تمامًا من الصفحة

---

## إخفاء العناصر مع إبقاء مكانها

- visibility: visible; (الوضع الافتراضي)
- visibility: hidden; (يخفي العنصر لكن يحافظ على مكانه)

---

## محاذاة النصوص في الوسط

### في HTML فقط

```sh
<center>النص في الوسط</center>
```

> ⚠️ تنسيق قديم غير مفضل – الأفضل استخدام CSS:

```sh
<body style="text-align: center;">
  المحتوى هنا
</body>
```

---

## استخدام التفاصيل / السرد التوضيحي

لإنشاء حاويات قابلة للطي مع عناوين مثل "About":

```sh
<details>
  <summary>About</summary>
  <p>هذه المعلومات تظهر عند الضغط</p>
  <img src="image.jpg">
  <br>
  <img src="image2.jpg">
</details>
```

---

## قوائم منسقة

### قائمة مرقمـة

```sh
<ol type="A">
  <li>Ahmed</li>
  <li>Ali</li>
</ol>
```

- type: 1، A، a، I، i

---

### قائمة غير مرقمـة

```sh
<ul type="square">
  <li>Home</li>
  <li>About</li>
</ul>
```

- type: disc، circle، square

---

### قائمة وصفيـة

```sh
<dl>
  <dt>HTML</dt>
  <dd>لغة هيكلة صفحات الويب</dd>
  <dt>CSS</dt>
  <dd>لغة تنسيق وتصميم الصفحات</dd>
</dl>
```

---

## عناصر قديمة وغير موصى بها (Deprecated)

- `<font>`: التحكم في الخطوط، الألوان، الأحجام
- `<center>`: تم الاستعاضة عنه بـ CSS
- bgcolor و align في الوسوم: يفضل استخدام CSS

---

## ملاحظات هامة

- بعض الخصائص القديمة لا تزال مدعومة لكن يفضل كتابة CSS في ملفات منفصلة.
- افصل الهيكل (HTML) عن التنسيق (CSS) لأفضل ممارسات التطوير.
- هذا الشرح يغطي أساسيات مهمة لكن ليس كل إمكانيات HTML. هناك وسوم متقدمة (video tracks، SVG، ARIA، إلخ) ودوال JavaScript للتفاعل.

---