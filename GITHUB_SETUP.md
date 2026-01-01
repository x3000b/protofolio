# تعليمات رفع المشروع إلى GitHub

## الخطوة 1: تثبيت Git

1. قم بتحميل Git من الموقع الرسمي: https://git-scm.com/download/win
2. قم بتثبيت Git على جهازك
3. أعد تشغيل Terminal/PowerShell بعد التثبيت

## الخطوة 2: تهيئة Git في المشروع

افتح Terminal في مجلد المشروع وقم بتنفيذ الأوامر التالية:

```bash
# تهيئة Git repository
git init

# إضافة جميع الملفات
git add .

# عمل commit أولي
git commit -m "Initial commit: Portfolio website"

# إضافة اسم المستخدم والبريد الإلكتروني (إذا لم تكن مضبوطة)
git config user.name "Your Name"
git config user.email "your.email@example.com"
```

## الخطوة 3: إنشاء Repository على GitHub

1. اذهب إلى https://github.com
2. سجل الدخول إلى حسابك (أو أنشئ حساب جديد)
3. انقر على زر "+" في الزاوية العلوية اليمنى
4. اختر "New repository"
5. أدخل اسم المستودع (مثلاً: "portfolio" أو "my-portfolio")
6. اختر Public أو Private
7. **لا تقم** بتهيئة README أو .gitignore (لأننا لدينا بالفعل .gitignore)
8. انقر على "Create repository"

## الخطوة 4: ربط المشروع بـ GitHub

بعد إنشاء المستودع على GitHub، ستظهر لك تعليمات. قم بتنفيذ الأوامر التالية (استبدل YOUR_USERNAME و YOUR_REPO_NAME):

```bash
# إضافة remote repository
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# تغيير اسم الفرع الرئيسي إلى main (إذا لزم الأمر)
git branch -M main

# رفع المشروع إلى GitHub
git push -u origin main
```

## ملاحظات مهمة:

- تأكد من عدم رفع الملفات الحساسة (مثل API keys)
- ملف `.gitignore` موجود بالفعل وسيتجاهل `node_modules` و `dist` تلقائياً
- بعد التعديلات المستقبلية، استخدم:
  ```bash
  git add .
  git commit -m "Your commit message"
  git push
  ```

