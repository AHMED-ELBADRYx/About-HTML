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

 ## لتحديد نوع المستند:
 ```sh
<!DOCTYPE html>
```

## كل الصفحة بعدها حتى النهاية يتم كتايتها بين:
```sh
<html>
</html>
```

## داخلها يوجد قسمين أساسيين:


### قسم لمعلومات الموقع يكون بين:
```sh
<head>
</head>
```

### قسم يظهر للمستخدم يكون بين:
```sh
<body>
</body>
```

---

# داخل رأس الموقع:

---

## لدعم أغلب اللغات ومنها العربية:
```sh
<meta charset="utf-8">
```

## لتحديد لغة الموقع نفسه فنكتبها في html:
```sh
<html lang="ar">
```

## لكتابة اسم الموفع تكون بين:
```sh
<title>
</title>
```

## لتحديد وصف الموقع:
```sh
<meta name="description" content="ما سيظهر للمستخدم في وصف الموقع">
```

## لظهور الموقع عند بحث معين:
```sh
<meta name="keywords" content="html , css , php">
```

## لتحديد صاحب الموقع:
```sh
<meta name="author" content="My name">
```

## لجعل الموقع متجاوبًا:
```sh
<meta name="viewport">
```

## لتحديث الموقع كل مدة معينة مثلا 3 ثواني:
```sh
<meta http-equive="refresh" content="3">
```

### مثلا إن انتقلنا لموقع جوجل خلال 4 ثواني تكون:
```sh
<meta http-equive="refresh" content="5" url=https://www.google.com/>
```

## للبحث عن كل أنواع الميتا اضغط [هنا](https://www.w3schools.com/tags/tag_meta.asp)

## لربط CSS خارجي:
```sh
<link rel="stylesheet" href="css/style.css">
```
- rel="stylesheet" : هو نوع علاقة الربط بملفات css
- href="css/style.css" : هو موقع الملف

## لكتابة CSS داخلي:
```sh
<style>
</style>
```

## لكتابة Java script داخلي:
```
<script>
</script>
```

---

# داخل جسم الموقع (body):

---

## الأوسمة تنقسم لقسمين:
- block: تنشئ سطرا جديدا (خاصة بالعناوين والفقرات)
- inline: تكون في نفس السطر (ختصة بتنسيق النصوص بدلا من css)

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

- 

---

## الروابط

- رابط أساسي:
```sh
<a href="https://example.com">رابط</a>
```

- فتح في نافذة جديدة:
```sh
<a href="https://example.com" target="_blank">رابط جديد</a>
```

- رابط تنزيل:
```sh
<a href="file.pdf" download="اسم الملف بعد التحميل">تحميل</a>
```

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
### يجب ان نكتب الصورة بمسارها الصحيح فنكتب اسمها فقط لو كانت داخل مجلد المشروع مباشرة أو لو كانت داخل المجلد فنكتبها كما هي داخل المجلد مثل "folder\img.jpg" أو لو كانت في مسار آخر أصلا فنكتب المسار كامل هكذا مثلا "D:\...\...\Images"

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

- border لتحديد سمك الحدود.
- colspan لدمج الأعمدة.
- rowspan لدمج الصفوف.
- thead, tbody, tfoot لتنظيم أقسام الجدول.

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

- الصور ستتوالى تحت بعضها باستخدام <br>.

---

## الحاويات

### حاوية عامة

```sh
<div>
  المحتوى هنا
</div>
```

- عنصر block، يأخذ عرض السطر بالكامل.

---

### عنصر داخل السطر

```sh
<span>نص صغير</span>
```

- عنصر inline، يبقى في السطر نفسه.

---

## إضافة فيديو وصوت

### فيديو

```sh
<video src="video.mp4" width="400" height="300" controls poster="cover.jpg">
  المتصفح لا يدعم الفيديو
</video>
```

- controls: لإظهار أزرار التشغيل
- poster: صورة مصغرة قبل التشغيل

---

### صوت

```sh
<audio src="sound.mp3" controls muted preload="auto">
  المتصفح لا يدعم الصوت
</audio>
```

- muted: كتم الصوت افتراضيًا
- preload:
  - auto: تحميل تلقائي
  - none: لا يتم التحميل إلا عند التشغيل
  - metadata: تحميل معلومات الملف فقط

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

```sh
<iframe src="https://example.com" width="500" height="300"></iframe>
```

- يستخدم لتضمين مواقع، فيديوهات، PDF... إلخ

---

### تضمين فيديو يوتيوب

- من اليوتيوب: كليك يمين على الفيديو → "نسخ رمز التضمين"
- النتيجة تكون مثل:

```sh
<iframe width="560" height="315"
src="https://www.youtube.com/embed/ID"
title="YouTube video" frameborder="0"
allowfullscreen></iframe>
```

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
  <input type="text" placeholder="اسم المستخدم"><br>
  <input type="password" placeholder="كلمة السر"><br>
  <input type="email" placeholder="البريد الإلكتروني"><br>
  <input type="number" placeholder="السن"><br>
  <input type="tel" placeholder="رقم الهاتف"><br>
  <input type="submit" value="تسجيل">
</form>
```

- placeholder: نص مساعد داخل الحقل

---

### أسئلة متعددة الاختيارات

```sh
<form>
  <p>ما هو لونك المفضل؟</p>
  <label><input type="radio" name="color" value="red" checked> أحمر</label><br>
  <label><input type="radio" name="color" value="blue"> أزرق</label><br>
  <input type="submit" value="إرسال">
</form>
```

- name نفسه لجعل الاختيارات حصرية
- checked لتحديد القيمة مبدئيًا

---

### مربعات اختيار (Checkbox)

```sh
<form>
  <label><input type="checkbox"> أوافق على الشروط</label><br>
  <input type="submit" value="إرسال">
</form>
```

---

### حقل نص طويل

```sh
<textarea rows="5" cols="30">اكتب رسالتك هنا...</textarea>
```

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

### قائمة مرقمة

```sh
<ol type="A">
  <li>Ahmed</li>
  <li>Ali</li>
</ol>
```

- type: 1، A، a، I، i

---

### قائمة غير مرقمة

```sh
<ul type="square">
  <li>Home</li>
  <li>About</li>
</ul>
```

- type: disc، circle، square

---

### قائمة وصفية

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

- <font>: التحكم في الخطوط، الألوان، الأحجام
- <center>: تم الاستعاضة عنه بـ CSS
- bgcolor و align في الوسوم: يفضل استخدام CSS

---

## ملاحظات هامة

- بعض الخصائص القديمة لا تزال مدعومة لكن يفضل كتابة CSS في ملفات منفصلة.
- افصل الهيكل (HTML) عن التنسيق (CSS) لأفضل ممارسات التطوير.
- هذا الشرح يغطي أساسيات مهمة لكن ليس كل إمكانيات HTML. هناك وسوم متقدمة (video tracks، SVG، ARIA، إلخ) ودوال JavaScript للتفاعل.

---

## نهاية الملف
