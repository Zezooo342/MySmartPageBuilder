# MySmartPageBuilder

منشئ صفحات (Page Builder) modular يسمح بتركيب مكوّنات (Components) لإنتاج صفحات HTML (ومستقبلاً قوالب React / Static Export) بسرعة ومرونة.

## الهدف (Goal)
توفير نواة (Core) وخط تجميع (Render Pipeline) يسمحان بتجميع عناصر قابلة لإعادة الاستخدام مع إعدادات (Props / Data Binding) وإخراج نظيف.

## الحالة الحالية (Status)
🚧 تأسيس البنية الأولية – لا يوجد منطق تنفيذي بعد.

## المزايا المخططة (Planned Features)
- مكونات جاهزة (Hero, Pricing, FAQ, CTA, Layout Grid).
- محرّك تجميع (Renderer) يدعم:
  - دمج Layout + Components
  - تمكين سمات (Theming) مستقبلًا
- دعم تصدير HTML ثابت (Static Export)
- دعم أوضاع متعددة (development / build)
- نظام قوالب (Template Packs)

## البنية المقترحة (Structure)
```
src/
  core/          # الأساس (Entity Models, Registry, Loader)
  components/    # المكونات القابلة لإعادة الاستخدام
  renderer/      # منطق التجميع والإخراج
tests/           # اختبارات لاحقًا
docs/            # توثيق معماري
```

## خارطة الطريق (Roadmap)
- [ ] تصميم نموذج المكوّن (Component Interface)
- [ ] إنشاء Registry للمكوّنات
- [ ] محرّك Renderer أولي يقبل JSON Schema
- [ ] ربط: إدخال → (تحليل) → (تجميع) → (إخراج HTML)
- [ ] دعم Slots داخل المكوّنات
- [ ] إضافة نظام قوالب جاهزة
- [ ] دعم Internationalization (i18n)
- [ ] دعم CLI بسيطة (build / preview)

## التشغيل مستقبلًا (Future Run)
سيتم لاحقاً إضافة CLI:
```
python -m venv venv
source venv/bin/activate   # على ويندوز: venv\Scripts\activate
pip install -r requirements.txt  # (لاحقاً)
python tools/dev_server.py
```

## المساهمة (Contributing)
انظر ملف CONTRIBUTING.md

## الأمان (Security)
لا تُرسل أسراراً في Issues عامة. اتبع إرشادات SECURITY.md.

## الترخيص (License)
MIT – انظر LICENSE.

---
**English Summary**
A modular page builder scaffold. Currently only the skeleton is being established. See roadmap for upcoming engine, component registry, and static export features.