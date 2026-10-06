# Naming Conventions — مشتق من Naming Tool.xlsx

> **⚠️ الحالة: غير مكتمل.** ملف `Naming Tool.xlsx` لم يصل بعد إلى بيئة العمل.
> لا يُعتمد أي جزء من هذا الملف كمصدر حتى تتم تعبئته من الملف الأصلي.
> **ممنوع إنشاء أي Campaign / Ad Set / Ad قبل اكتمال هذا الملف.**

---

## القاعدة الأساسية

اسم الـ Ad يُستخدم **حرفيًا وبدون أي تعديل** داخل ثلاث معاملات في الرابط:

| المعامل | المصدر |
|---|---|
| `source` | اسم الـ Ad — مطابقة 100% |
| `utm_source` | اسم الـ Ad — مطابقة 100% |
| `utm_campaign` | اسم الـ Ad — مطابقة 100% |
| `prod_category` | **من `Naming Tool.xlsx` فقط** — ممنوع التخمين |

### مثال معتمد

اسم الـ Ad:

```
SNPC_Purifier7_arp_VDO_SA_2026Q2_V3
```

الرابط:

```
https://naqi.sa/order/?source=SNPC_Purifier7_arp_VDO_SA_2026Q2_V3&utm_source=SNPC_Purifier7_arp_VDO_SA_2026Q2_V3&utm_campaign=SNPC_Purifier7_arp_VDO_SA_2026Q2_V3&prod_category=airpurifier7
```

### بنية الاسم كما تظهر في المثال

```
<Platform>_<Product>_<ProductCode>_<Format>_<Market>_<Period>_<Version>
   SNPC     Purifier7     arp         VDO       SA      2026Q2      V3
```

> هذا **استنتاج من مثال واحد فقط**، وليس مرجعًا. القيم المعتمدة لكل خانة
> (اختصارات المنصات، المنتجات، الـ Formats، الأسواق، الفترات) تُنقل من
> `Naming Tool.xlsx` ولا تُجتهد.

---

## جدول prod_category

| المنتج | prod_category |
|---|---|
| Purifier 7 (من المثال أعلاه) | `airpurifier7` |
| _(بقية القيم — تُنقل من Naming Tool.xlsx)_ | |

---

## Checklist قبل نشر أي إعلان

- [ ] الاسم مبني حسب القواعد المعتمدة في `Naming Tool.xlsx`
- [ ] `source` = اسم الـ Ad بالحرف
- [ ] `utm_source` = اسم الـ Ad بالحرف
- [ ] `utm_campaign` = اسم الـ Ad بالحرف
- [ ] `prod_category` منقولة من الملف (ليست مكتوبة يدويًا)
- [ ] الرابط مفحوص بالكامل قبل النشر
