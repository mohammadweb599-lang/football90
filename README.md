project-root/
│
├── /public/                    # فایل‌های استاتیک و عمومی
│   ├── /images/               # تصاویر بهینه‌شده (WebP)
│   │   ├── coach.webp
│   │   ├── tactic-board.webp
│   │   ├── icons/            # آیکون‌ها (زنگوله، سکه، نمودار)
│   │   │   ├── bell.webp
│   │   │   ├── coin.webp
│   │   │   ├── chart.webp
│   │   └── ...
│   ├── index.html            # فایل HTML اصلی
│   └── favicon.ico
│
├── /src/                      # کد منبع فرانت‌اند
│   ├── /components/          # کامپوننت‌های React قابل استفاده مجدد
│   │   ├── Header.tsx
│   │   ├── TacticBoard.tsx
│   │   ├── Menu.tsx
│   │   ├── PlayerCard.tsx    # برای فروشگاه
│   │   └── ...
│   ├── /pages/              # صفحات مختلف (18 صفحه طراحی‌شده)
│   │   ├── Home.tsx         # صفحه اصلی
│   │   ├── AdminDashboard.tsx
│   │   ├── Shop.tsx         # صفحه فروشگاه
│   │   ├── Tactic.tsx       # صفحه ترکیب و تاکتیک
│   │   ├── Profile.tsx      # صفحه پروفایل (/profile/:username)
│   │   ├── Stats.tsx        # صفحه آمار
│   │   ├── Support.tsx      # صفحه پشتیبانی
│   │   └── ...
│   ├── /services/           # سرویس‌ها برای API و منطق
│   │   ├── authService.ts   # احراز هویت (JWT)
│   │   ├── paymentService.ts # درگاه زرین‌پال
│   │   ├── gameService.ts   # شبیه‌سازی بازی
│   │   └── ...
│   ├── /utils/              # ابزارهای کمکی
│   │   ├── imageOptimizer.ts # بهینه‌سازی تصاویر
│   │   └── constants.ts     # ثابت‌ها (مثل نقش‌ها، تاکتیک‌ها)
│   ├── /styles/             # استایل‌ها
│   │   ├── global.css       # استایل‌های سراسری
│   │   └── tailwind.css
│   ├── App.tsx              # کامپوننت اصلی اپلیکیشن
│   ├── index.tsx            # نقطه ورود اپلیکیشن
│   └── types.ts             # تعریف تایپ‌ها برای TypeScript
│
├── /server/                  # کد منبع بک‌اند (Node.js)
│   ├── /config/             # تنظیمات
│   │   ├── db.ts            # اتصال به MongoDB
│   │   └── env.ts           # متغیرهای محیطی (مثل کلید زرین‌پال)
│   ├── /models/             # مدل‌های دیتابیس
│   │   ├── User.ts
│   │   ├── Player.ts
│   │   ├── Team.ts
│   │   └── ...
│   ├── /routes/             # مسیرهای API
│   │   ├── authRoutes.ts    # ثبت‌نام، ورود
│   │   ├── paymentRoutes.ts # درگاه پرداخت
│   │   ├── gameRoutes.ts    # شبیه‌سازی بازی
│   │   └── ...
│   ├── /controllers/        # کنترلرها
│   │   ├── authController.ts
│   │   ├── paymentController.ts
│   │   └── ...
│   ├── /middleware/         # میدل‌ورها
│   │   ├── authMiddleware.ts # احراز هویت
│   │   └── ...
│   ├── server.ts            # نقطه ورود سرور
│   └── cronJobs.ts          # زمان‌بندی (Cron Jobs برای سکه و لیگ‌ها)
│
├── /docs/                    # مستندات
│   ├── architecture.md      # معماری پروژه
│   ├── setup-guide.md       # راهنمای راه‌اندازی
│   └── api-spec.md          # مشخصات API
│
├── /tests/                   # تست‌ها
│   ├── /unit/               # تست‌های واحد
│   │   ├── auth.test.ts
│   │   └── ...
│   └── /integration/        # تست‌های یکپارچه
│       └── game.test.ts
│
├── .env                      # متغیرهای محیطی (کلیدها، پورت‌ها)
├── .gitignore                # فایل‌های نادیده‌گرفته‌شده
├── package.json             # وابستگی‌ها و اسکریپت‌ها
├── tsconfig.json            # تنظیمات TypeScript
├── tailwind.config.js       # تنظیمات Tailwind CSS
└── README.md                # راهنمای اولیه پروژه# football90
