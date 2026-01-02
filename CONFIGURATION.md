# ⚙️ تعليمات التكوين والتحديثات

## 📋 التحديثات المطلوبة للموقع

### 1️⃣ **تحديث معلومات التواصل**

#### في ملف `js/script.js`:

**استبدل رقم WhatsApp:**
```javascript
// البحث عن هذا السطر:
let whatsappURL = `https://wa.me/201014499448?text=${encodeURIComponent(whatsappMessage)}`;

// واستبدله برقمك:
let whatsappURL = `https://wa.me/YOUR_WHATSAPP_NUMBER?text=${encodeURIComponent(whatsappMessage)}`;
```

**استبدل بريدك الإلكتروني:**
```javascript
// البحث عن هذا السطر:
let mailtoLink = `mailto:contact@jokerel3arab.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;

// واستبدله ببريدك:
let mailtoLink = `mailto:YOUR_EMAIL@gmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
```

### 2️⃣ **تحديث روابط السوشيال ميديا**

#### في ملف `index.html`:

**في قسم Footer (البحث عن Social Icons):**
```html
<!-- استبدل الروابط:-->
<a href="https://wa.me/YOUR_WHATSAPP_NUMBER" target="_blank" class="text-warning text-decoration-none">
    <i class="fab fa-whatsapp fa-lg"></i>
</a>
<a href="mailto:YOUR_EMAIL@gmail.com" class="text-warning text-decoration-none">
    <i class="fas fa-envelope fa-lg"></i>
</a>
<a href="https://www.facebook.com/YOUR_FACEBOOK_PAGE" target="_blank" class="text-warning text-decoration-none">
    <i class="fab fa-facebook fa-lg"></i>
</a>
<a href="https://www.instagram.com/YOUR_INSTAGRAM_HANDLE" target="_blank" class="text-warning text-decoration-none">
    <i class="fab fa-instagram fa-lg"></i>
</a>
```

**أيضاً في قسم Home (الأسفل):**
```html
<!-- في Social Media Section:-->
<a href="https://wa.me/YOUR_WHATSAPP_NUMBER" target="_blank"><i class="fab fa-whatsapp"></i></a>
<a href="https://www.facebook.com/YOUR_FACEBOOK_PAGE" target="_blank"><i class="fab fa-facebook-f"></i></a>
<a href="https://www.instagram.com/YOUR_INSTAGRAM_HANDLE" target="_blank"><i class="fab fa-instagram"></i></a>
<a href="https://www.linkedin.com/in/YOUR_LINKEDIN_PROFILE" target="_blank"><i class="fab fa-linkedin-in"></i></a>
```

### 3️⃣ **تحديث معلومات عنك**

#### في قسم "About Me":
```html
<!-- استبدل المعلومات الشخصية -->
I am Youssef Hesham, also known as Joker_el3arab...
```

### 4️⃣ **إضافة صورة CV (اختياري)**

ضع ملف `Youssef_CV.pdf` في المجلد الرئيسي (بجانب `index.html`)

---

## 🖼️ تحديث الصور

### الصور المستخدمة حالياً:
- `./Imge/joker_el3arab7.jpg` - صورة الملف الشخصي في Hero
- `./Imge/joker.png` - صورة في About و Footer
- `./Imge/1f.jpg` و `./Imge/2f.jpg` - صور العملاء في Testimonials
- صور Portfolio في مجلد `Imge/`

### ملاحظات عن الصور:
- تأكد من أن جميع الصور موجودة في مجلد `Imge/`
- استخدم صور عالية الجودة
- الصور في Portfolio يجب أن تكون بنفس النسبة (مربعة أو مستطيلة)

---

## 🎨 تخصيص الألوان

### في ملف `css/style.css`:

```css
:root {
    --black: rgb(0, 0, 0);           /* اللون الأسود الأساسي */
    --white: white;                  /* الأبيض */
    --dark-cyan: #ffcc00;            /* اللون الذهبي (الأساسي) - غيّره هنا */
    --dark: #000;                    /* الأسود الداكن */
    --second: #0c0c0c;               /* خلفية ثانوية */
    --accent: #ff6b6b;               /* اللون الإضافي */
}
```

**مثال لتغيير اللون الذهبي إلى أزرق:**
```css
--dark-cyan: #00D4FF;  /* أزرق فاتح */
```

---

## 📱 اختبار الموقع

### طرق الاختبار:

1. **في المتصفح:**
   - اضغط F12 لفتح Developer Tools
   - انقر على Device Toggle (أيقونة الهاتف)
   - اختبر على أحجام مختلفة

2. **الأجهزة:**
   - الكمبيوتر (1920px+)
   - الجهاز اللوحي (768px)
   - الهاتف (375px+)

3. **المتصفحات:**
   - Chrome
   - Firefox
   - Safari
   - Edge

---

## ✅ قائمة التحقق قبل النشر

- [ ] تحديث رقم WhatsApp
- [ ] تحديث البريد الإلكتروني
- [ ] تحديث روابط السوشيال ميديا
- [ ] تحديث معلومات البروفايل
- [ ] إضافة جميع صور Portfolio
- [ ] اختبار نموذج التواصل
- [ ] اختبار الموقع على الهاتف
- [ ] اختبار جميع الروابط
- [ ] التحقق من الأداء (Page Speed)

---

## 🚀 نشر الموقع

### المنصات الموصى بها:
1. **Netlify** - مجاني وسهل
2. **Vercel** - أداء ممتاز
3. **GitHub Pages** - مجاني (Git مطلوب)
4. **Hostinger** - استضافة مدفوعة موثوقة

### خطوات النشر على Netlify:
1. انسخ جميع الملفات (index.html, css, js, Imge)
2. اذهب إلى https://netlify.com
3. اسحب المجلد على الموقع
4. سيتم نشر الموقع مباشرة!

---

## 🔧 استكشاف الأخطاء

### لا تظهر الأنيميشنات:
- تحقق من أن ملفات CSS و JS محملة بشكل صحيح
- افتح Console (F12) وابحث عن أخطاء

### لا يعمل زر التواصل:
- تحقق من رقم WhatsApp صحيح
- تأكد من أن JavaScript مفعّل

### الصور لا تظهر:
- تحقق من أن مجلد `Imge/` موجود
- تأكد من أسماء الملفات صحيحة (حساس للأحرف الكبيرة والصغيرة)

---

## 📞 الدعم الفني

للمزيد من المساعدة:
- تحقق من جميع الروابط في `index.html`
- استخدم Developer Tools (F12) لاكتشاف الأخطاء
- اختبر على متصفحات مختلفة

---

**آخر تحديث:** 22 نوفمبر 2025
