# تعليمات نسخ المشروع

## الملفات المطلوبة للنسخ:

### 1. ملفات التكوين الرئيسية:
- package.json
- vite.config.ts  
- tailwind.config.ts
- tsconfig.json
- components.json
- drizzle.config.ts
- postcss.config.js
- README.md
- .gitignore

### 2. مجلد client/
- client/index.html
- client/src/App.tsx
- client/src/main.tsx
- client/src/index.css
- client/src/components/video-extractor-form.tsx
- client/src/components/video-result.tsx
- client/src/hooks/use-mobile.tsx  
- client/src/hooks/use-toast.ts
- client/src/lib/queryClient.ts
- client/src/lib/utils.ts
- client/src/pages/home.tsx
- client/src/pages/not-found.tsx

### 3. مجلد server/
- server/index.ts
- server/routes.ts
- server/storage.ts
- server/vite.ts

### 4. مجلد shared/
- shared/schema.ts

## بعد النسخ:
1. أنشئ مجلد جديد على جهازك
2. انسخ كل الملفات بنفس التسلسل
3. افتح terminal في مجلد المشروع
4. نفذ: npm install
5. أضف ملف .env وحط فيه: YOUTUBE_API_KEY=مفتاحك
6. نفذ: npm run dev

## للرفع على GitHub:
git init
git add .
git commit -m "YouTube metadata extractor"
git remote add origin <repository-url>
git push -u origin main