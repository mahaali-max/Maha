# Naqi — Paid Media Workspace

مرجع العمل لإدارة حملات نقي المدفوعة عبر Whathead MCP.

## قواعد إلزامية (لا استثناءات)

### 1. الـ Naming قبل أي إنشاء
- ممنوع إنشاء أي **Campaign** أو **Ad Set** أو **Ad** قبل مراجعة `memory/naming.md`
  (المشتق من `Naming Tool.xlsx`) والتأكد أن التسمية مطابقة للقواعد المعتمدة.
- اسم الـ Ad يجب أن يطابق **100%** قيم `source` و `utm_source` و `utm_campaign` في الرابط.
- قيمة `prod_category` تؤخذ **فقط** من ملف المسميات — ممنوع تخمينها أو كتابتها من الذاكرة.
- يتم فحص الرابط والتسمية **قبل** نشر الإعلان.

مثال معتمد — اسم الإعلان:

```
SNPC_Purifier7_arp_VDO_SA_2026Q2_V3
```

الرابط المقابل له:

```
https://naqi.sa/order/?source=SNPC_Purifier7_arp_VDO_SA_2026Q2_V3&utm_source=SNPC_Purifier7_arp_VDO_SA_2026Q2_V3&utm_campaign=SNPC_Purifier7_arp_VDO_SA_2026Q2_V3&prod_category=airpurifier7
```

> أي اختلاف ولو بسيط يكسر الـ Tracking والـ Attribution والتقارير.

### 2. مراجعة القديم قبل بناء الجديد
قبل إنشاء أي حملة جديدة، راجع الحملات الشغّالة أو اللي حققت نتائج قوية على نفس
الحساب، وافهم: بناء الـ Campaign، تقسيم الـ Ad Sets، الـ Objective، الـ Audiences،
الـ Placements، الـ Optimization Event، توزيع الميزانية، الـ Bidding Strategy،
الـ Creatives والـ Formats، الـ Copy، الـ URLs والـ UTMs، والـ Naming Convention.
أي شيء ناجح يُكتشف أثناء المراجعة يُضاف فورًا إلى `memory/playbook.md`.

### 3. Native Tools أولًا
استخدم الـ native tools الخاصة بكل منصة قدر الإمكان
(`meta_native_action`، `tiktok_native_action`، `snapchat_native_action`)
بدل الأدوات العامة.

## خريطة الملفات

| الملف | المحتوى |
|---|---|
| `memory/accounts.md` | الحسابات المربوطة على كل المنصات + الـ IDs |
| `memory/naming.md` | الـ Naming Conventions وقيم `prod_category` |
| `memory/playbook.md` | Knowledge Base للحملات والإعدادات اللي نجحت |
