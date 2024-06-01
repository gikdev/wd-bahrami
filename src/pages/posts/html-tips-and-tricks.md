---
id: 000
layout: ../../layouts/Post.astro
title: چند تا ترفند HTML
date: ۱۴۰۳/۰۳/۰۸
theme: secondary
draft: false
---

## صفت `start`

این صفت کمک میکنه که بتونید برای شماره شروع لیست‌ها رو تنظیم کنید.

```html
<ol start="20">
  <li>Pineapple🍍</li>
  <li>Apple🍎</li>
  <li>Greenapple 🍏</li>
</ol>
```


![نتیجه کد بالا](https://wd-bahrami.storage.iran.liara.space/images/ik05u8a96h506u314ubm.png)

---

## صفت `contenteditable`

این صفت رو اگه مقدار `true` بهش بدید محتوای اون المان قابل ویرایش میشه.

```html
<p contenteditable="true">It can be something about you.</p>
```


![نتیجه کد بالا](https://wd-bahrami.storage.iran.liara.space/images/3j7fbm6l7mjuy552immb.gif)

---

## صفت `required`

این صفت رو روی هر تگ `input` بذارین باعث میشه که کاربر مجبور به پرکردن اون بشه.

```html
<input type="password" required />
```

---

## تگ `mark`

با این میتونین متن رو هایلایت کنین!

```html
<p>This is <mark>important</mark></p>
```

![نتیجه کد بالا](https://wd-bahrami.storage.iran.liara.space/images/1tpq69elepymsveoi4dd.png)

---

## صفت `loading`

اگه مقدار این صفت رو `lazy` گذاشته باشین (روی المان‌های رسانه‌ای)، باعث میشه که تا وقتی که کاربر بهشون نرسیده، اون عکس یا ... لود نشه

```html
<img src='image.jpg' loading='lazy' alt='Alternative text'>
```

---

## تگ `kbd`

اگه میخواین دکمه های کیبورد رو نمایش بدین از این تگ استفاده کنین.

```html
<p>Press <kbd>alt</kbd> & <kbd>tab</kbd> to change window</p>
```
![نتیجه کد بالا](https://wd-bahrami.storage.iran.liara.space/images/t9fd85bnbgban8o9mevr.png)

---

## تگ‌های `details` و `summary`

این ۲ تگ بهتون کمک میکنن که المان کرکره‌ای (accordion) بسازین:

```html
<details>
  <summary>Can i save and love ❤️ this article?</summary>
  <p>Follow on twitter for more stuff.</p>
  <p>Save for updates.</p>
</details>
```

![نتیجه کد بالا](https://wd-bahrami.storage.iran.liara.space/images/xpfv1roxs2nmtky2z2y2.gif)

---

## صفت `accept`

این صفت برای اینه که مشخص بشه چه نوع فایل‌هایی میتونن آپلود بشن.

```html
<input type="file" accept=".jpg, .pdf">
```

---

## عکس `favicon`

در واقع `favicon` همون عکسی هستش که در تب مرورگر کنار اسم سایت نمایش داده میشه... این رو میشه با تگ `link` درست کرد.

```html
<link rel="icon" href="logo.webp">
```

---

## تگ `picture`

این تگ بهتون اجازه میده که عکس‌های متفاوتی رو براساس اندازه و نوع صفحه نمایش نشون بدین که برای طراحی واکنشگرا معرکه هست!

```html
<picture>
  <source srcset="large.webp" media="(min-width: 1200px)">
  <source srcset="medium.webp" media="(min-width: 800px)">
  <img src="regular.jpg" />
</picture>
```

---

## صفت `dir`

با کمک این صفت شما میتونین جهت سایت، متن و ... رو تنظیم کنین، اگر هم مقدار رو خودکار بذارین خودش بصورت خودکار با توجه به زبان تنظیم میشه.

```html
<p dir="rtl">Awesome!</p>
```

---

## صفت `spellcheck`
اگه میخواین غلط‌های املایی رو پیدا کنین، این بدردتون میخوره

```html
<input type="text" id="comment" spellcheck="true" />
```

---

## تگ متا (`<meta />`) از نوع `description`

این رو باید توی تگ `<head>` تون بذارین که توی موتورهای جستجو زیر اسم و دامنه سایت نمایش داده میشه و توضیح اون صفحه یا وبسایتتون هست...

```html
<meta name="description" content="Gitpod streamlines developer workflows by providing prebuilt, collaborative developer environments in your browser - powered by VS Code.">
```

![نتیجه کد بالا](https://wd-bahrami.storage.iran.liara.space/images/zr5wfg018xoq6ficpods.png)

---

## تگ `abbr`

تگ `abbr` برای نمایش دادن کلمات مختصر به کار میره. به طوری که اگه ماوس رو روی اون کلمه نگه دارین مقدار صفت `title` این تگ به صورت تولتیپ (`tooltip`) نمایش داده میشه

```html
<abbr title="National Aeronautics and Space Administration">NASA 🚀</abbr>
```

---

## صفت `disabled`

این صفت به هر المان فرمی داده بشه **غیرفعال**‌ میشه.

```html
<select>
  <option>HTML</option>
  <option>CSS</option>
  <option disabled>REACT</option>
</select>
```

---

## صفت `poster`

برای اینکه تا ویدیوتون لود میشه روی اون کاوری نمایش داده بشه که میتونین با صفت `poster` تنظیمش کنین.

```html
<video src="video.mp4" poster="flowers.jpg"></video>
```

---

## صفت `reversed`

اگه این رو روی تگ `ol` بذارین، شمارش رو از آخر لیست شروع میکنه.

```html
<ol reversed>
  <li>Pineapple🍍</li>
  <li>Apple🍎</li>
  <li>Greenapple 🍏</li>
</ol>
```

![نتیجه کد بالا](https://wd-bahrami.storage.iran.liara.space/images/pk5mrp4qg0ahv8l448qx.png) 

---

امیدوارم که از خوندن این مقاله لذت برده باشین. کد خوبی داشته باشین!!! ✨❤️

نویسنده: سید محسن رضا (Syed Mohsin Raza)  
مترجم: محمد‌مهدی بهرامی  
منبع (مقاله اصلی): [HTML Tips & Tricks](https://dev.to/devsyedmohsin/html-tips-tricks-that-you-will-love-to-know-27ig)