# مستخرج معلومات يوتيوب

موقع ويب لاستخراج معلومات الفيديوهات من يوتيوب باللغة العربية

## المميزات

- ✅ استخراج الصورة المصغرة بجودة عالية (1920×1080)
- ✅ الحصول على عنوان الفيديو
- ✅ عرض مدة الفيديو
- ✅ تحميل الصور مباشرة
- ✅ واجهة عربية بتصميم RTL

## التقنيات المستخدمة

- **Frontend**: React + TypeScript + Vite
- **Backend**: Node.js + Express
- **UI**: Tailwind CSS + Shadcn/UI
- **API**: YouTube Data API v3

## التشغيل المحلي

1. انسخ المشروع:
```bash
git clone <repository-url>
cd youtube-metadata-extractor
```

2. تثبيت المكتبات:
```bash
npm install
```

3. إنشاء ملف `.env` وإضافة مفتاح YouTube API:
```
YOUTUBE_API_KEY=your_api_key_here
```

4. تشغيل المشروع:
```bash
npm run dev
```

## الحصول على مفتاح YouTube API

1. اذهب إلى [Google Cloud Console](https://console.cloud.google.com)
2. أنشئ مشروع جديد
3. فعّل YouTube Data API v3
4. أنشئ مفتاح API
5. أضف المفتاح في متغيرات البيئة

## النشر

يمكنك نشر الموقع على:
- Render (مجاني)
- Railway (500 ساعة مجانية)
- Vercel (مع تعديلات بسيطة)

## الترخيص

MIT License