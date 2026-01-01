# خطوات رفع الملفات إلى GitHub

المستودع موجود على GitHub لكن الملفات لم تُرفع بعد. اتبع هذه الخطوات:

## الطريقة 1: استخدام GitHub Desktop (الأسهل)

1. افتح **GitHub Desktop**
2. انقر على **File** > **Add Local Repository**
3. اختر مجلد المشروع: `C:\Users\dmush\OneDrive\Desktop\my works\protofolio - Copy`
4. إذا ظهرت رسالة "This directory does not appear to be a Git repository":
   - انقر على **"create a repository"** أو **"create a repository here"**
   - اترك الإعدادات الافتراضية
   - انقر **Create Repository**
5. بعد ذلك، سترى جميع الملفات في GitHub Desktop
6. في الأسفل، اكتب رسالة commit مثل: "Add portfolio website files"
7. انقر على **Commit to main**
8. انقر على **Publish repository** أو **Push origin** (إذا كان المستودع مربوطاً بالفعل)
9. اختر المستودع: `x3000b/protofolio---Copy`
10. انقر **Push**

## الطريقة 2: استخدام Terminal (إذا كان Git مثبت)

افتح Terminal في مجلد المشروع ونفذ:

```bash
git init
git add .
git commit -m "Add portfolio website files"
git branch -M main
git remote add origin https://github.com/x3000b/protofolio---Copy.git
git push -u origin main
```

## ملاحظة

إذا واجهت مشكلة في ربط المستودع، يمكنك:
- في GitHub Desktop: Repository > Repository Settings > Remote > Change remote URL
- أو حذف المستودع المحلي وإعادة إضافته من GitHub

