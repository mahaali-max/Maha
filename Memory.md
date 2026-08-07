# Memory.md — قاعدة المعرفة التسويقية لـ NAQI (Marketing Knowledge Base)

> **آخر تحديث:** 2026-08-05
> **الغرض:** هذا الملف هو المرجع الرئيسي لكل ما أثبت نجاحه في حملات نقي الإعلانية (Meta / TikTok / Snapchat / …).
> أي Campaign / Ad Set / Ad يحقق نتائج جيدة، أو أي Setup / Strategy / Best Practice ناجحة، **يُوثَّق هنا فوراً**.
> الهدف: نرجع له عند بناء حملات جديدة، نستخدمه كـ Payload جاهز، نسرّع التنفيذ، نقلل الأخطاء، ونكرر ما نجح بدل البدء من الصفر كل مرة.

---

## 0) القواعد الثابتة (Standing Rules) — تُطبَّق على كل عمل مستقبلي بدون استثناء

1. **الأولوية دائماً لـ Native Tools الخاصة بكل منصة** (مثل `snapchat_campaigns_campaign_id_adsquads_get`, `snapchat_adsquads_ad_squad_id_ads_get`, `snapchat_*_stats_report`) بدلاً من الأدوات العامة الموحّدة (`list_campaigns`, `fetch_*`) — إلا إذا لم يوجد مقابل Native للمهمة المطلوبة.
2. **لا يتم إنشاء أي Campaign / Ad Set / Ad جديد قبل مراجعة الحملات القديمة على نفس الحساب** — خصوصاً الحملات/الـAd Sets/الـAds التي ما زالت تعمل (`ACTIVE`) أو التي أثبتت نتائج قوية سابقاً. الحملات القديمة الناجحة = المرجع العملي الأساسي؛ لا تُغيَّر الإعدادات أو يُبدأ من الصفر بدون سبب واضح.
3. **الالتزام الحرفي بملف `Naming Tool.xlsx`** كمرجع وحيد لكل Naming Convention و prod_category. لا تخمين، لا كتابة يدوية من الذاكرة، لا اختصار خارج القواعد المعتمدة.
4. **قاعدة لا تقبل الاستثناء:** اسم الـ Ad = قيمة `source` = قيمة `utm_source` = قيمة `utm_campaign` بنسبة 100%. وقيمة `prod_category` في الرابط تُؤخذ فقط من عمود `prod_category (URL)` في الشيت.
5. **فحص الرابط والتسمية إلزامي قبل نشر أي إعلان.**
6. كل حالة ناجحة جديدة تُضاف إلى القسم 4 من هذا الملف بنفس القالب المستخدم أدناه.

---

## 1) ملخص Naming Tool.xlsx (Snapshot بتاريخ 2026-08-05)

> ⚠️ الملف الأصلي (`Naming Tool.xlsx`) هو **المصدر الوحيد المعتمد**. هذا القسم نسخة قراءة سريعة فقط — عند أي تحديث على الشيت الأصلي يجب إعادة مزامنة هذا القسم.

### 1.1 الأكواد الأساسية (Sheet1 / Sheet2 — متطابقتان)

| البُعد | القيم → الكود |
|---|---|
| **Brand** | Naqi → `Naqi` |
| **Channel** | Social_Media→SOC · Display→DIS · Video→VID · Programmatic→PRG · BSP→BSP · Search→SEM · Influencer→INFR |
| **Medium** | Twitter→TWT · **Snapchat→SNPC** · Facebook→FBK · Tiktok→TKK · Instagram→ING · Youtube→YTBE · Tabby→TABBY · Tamara→TAMARA · Amazon→AMZ · GDN→GDN · Search→SRCH · DV360→DV360 · Affiliates→AFFS · Noon→NOON · Influencer→INFR · Bio links: TTBIO / SNPBIO / FABBIO / TTKKBIO / INBIO / YTBIO |
| **Country** | Saudi_Arabia→SA · United_Arab_Emarites→UAE · Bahrain→BA |
| **Funnel Stage** | Awarness→AWA · Consideration→CONS · Conversion→CONV · Loyalty→LOYL · Revenue→REV |
| **Objective** | Reach→RCH · Conversion→CONV · Brand Awareness→BR-AW · Post Engagement→PST-ENG · Video Views→VID-VIEW · Link Click→LNK-CL · Landing Page View→LP-VIEW · Product Catalog→PROD-CAT · Lead Generation→LEAD-GEN · Purchase→PUR · Retargeting Visitors→RET-VIS |
| **City** | Riyadh→RYD · Jiddah→JED · Makkah→MKH · Madinah→MDN · Dammam→DMM · Khobar→KHB · Taif→TIF · Tabuk→TBK · Buraydah→BRD · Al-Ahsa→AHS · Najran→NJR · Jubail→JBL · Yanbu→YNB · Abha→AHB · Hail→HIL · NA→NA |
| **Targeting** | Retargeting→RT · Lookalike→LAL · Interest→INT · Geographic→GEO · Gender Male→GENM · Gender Female→GENF · Affinity→AFF · In Market→INM |
| **Ad Format** | Video→VDO · Image→IMG · Carousel→CRSL · DCO→DCO · Dynamic→DYNM · Text→TEXT |
| **Department** | Installation→Install · Deleviry→Deleviry |
| **Product Category** | Water Filters→wtrflt · Self-Cooling Dispenser→scd · Filtered Dispenser→fltD · Ice cream→icm · Ice Makers→icmkr · Coffee Machines→cfm · Beverage Machine→bvm · Heater→htr · Refrigerators→rfr · mist→mst · Fogging Machines→fgm · Air Purifiers→arp · recycling→rcyc · Airhumidifier→ahm · Pumps→pmp · Spare Parts & Accessories→spa · packages→pkg · Kitchen Products→KTP · Others→oth · B2B→B2B · Franchise Partner Acquisition→FranchiseAcquisition · Franchise Branch→FranchiseBranch · summerGeneric→summerGeneric |

### 1.2 جدول المنتجات الكامل (Product Name → Product Code (Name in Ad) → prod_category للرابط)

> الأعمدة P/Q/R في الشيت. **هذا هو الجدول الذي يُستخدم فيه `Product Code` داخل اسم الـ Ad، وقيمة `prod_category` داخل الرابط.**

| Product Name (AR) | Product Code (بالـ Ad) | prod_category (URL) |
|---|---|---|
| فلتر سلفر كيو | Fltrslvrq | silverQ7stages |
| فلتر سلفر كيو + خلاط مزدوج | fltrkitchdblefaucet | fltrkitchdblefaucet |
| فلتر ديرتنا | filterdrtna | filterdrtna |
| نقي بلاك اديشن 100 جالون | Fltrblk | blackq |
| فلتر نقي المتنقل | tripfilter | tripfltr |
| الصندوق الأزرق | bluebox | bluebox |
| نقي ديجيتال 75جالون | digital75 | digital75 |
| فلتر كينت اكسيل | kentexcellplus | kentexcellplus |
| فلتر كينت جراند بلص | kentgrand | kentgrand |
| فلتر كينت برايم | kentprime | kentprime |
| فلتر جامبو | Fltrjmb | Jumbofilter |
| برادة S | Clrs | coolers |
| برادة R1 | Clrr1 | coolerR1 |
| برادة P1 | Clrp1 | coolerP1 |
| برادة H1 | Clrh1 | coolerH1 |
| برادة نقي زر أمان | Clrsafe | coolersafe |
| برادة نقي بزر أمان المطورة | Clrsafe | coolersafe |
| برادة نقي بفلتر داخلي زجاجية فاخرة | Clrgls | procoolergls |
| برادة نقي شكل ماكينة قهوة | Clrcoffee | coolercoffe |
| برادة فاخرة بلس | Clrext | coolerext |
| البرادة الذكية برو | smartclrpro | smartcoolerpro |
| البرادة الذكية | smartclr | smartcooler |
| برادة نقي أكسترا بلس | Clrext | coolerext |
| برادة نقي برو بفلتر داخلي | proclrpro | procoolerpro |
| برادة نقي برو بلس بفلتر داخلي | proclrpls | procoolerpls |
| برادة نقي مفلترة E | Clre | coolerE |
| برادة نقي مفلترة D | Clrd | coolerD |
| برادة نقي مفلترة M | Clrm | coolerM |
| برادة نقي مفلترة U1 | Clru1 | coolerU1 |
| صانعة آيس كريم اسود | icecream | icecream |
| صانعة ايس كريم N1 | IcecreamN1 | icecreamN1 |
| صانعة ايس كريم C1 | icecreamC1 | icecreamC1 |
| صانعة الثلج - كلاسيك | Iceclassic | icemakerclass |
| صانعة الثلج - بريميوم | iceprem | icemakerprem |
| صانعة الثلج - برو | Icepro | icemakerpro |
| صانعة الثلج - سمارت | Icesmart | icemakersmrt |
| صانعة مكعبات الثلج - L2 | IceL2 | IceL2 |
| قهوة نقي المقطرة | coffeenaqi | coffeenaqi |
| قهوة نقي المختصة Cor1 | coffeenaqi2 | coffeenaqi2 |
| ركن القهوة | coffeecorner | coffeecorner |
| مطحنة قهوة | coffeeGrinder | coffeeGrinder |
| آلة المشروبات الساخنة 10 لتر | dirnkhot10 | dirnkhot10 |
| آلة المشروبات الساخنة 5 لتر | dirnkhot5 | dirnkhot5 |
| دفاية داخلية كلاسيك | heaterclass | heaterclass |
| دفاية داخلية بريميوم | heaterprem | heaterprem |
| دفاية نقي برو | naqiheaterpro | naqiheaterpro |
| دفاية نقي | naqiheater | naqiheater |
| ثلاجة متنقلة كلاسيك | boxclass | boxclass |
| ثلاجة متنقلة برو | boxfpro | boxfpro |
| ثلاجة متنقلة برو بلس | boxproplus | boxproplus |
| ثلاجة متنقلة بريميوم | boxprem | boxprem |
| ثلاجة متنقلة بريميوم بلس | boxpremplus | boxpremplus |
| واجهة تبريد نقي 90 لتر | cold90 | cold90 |
| واجهة تبريد نقي 70 لتر | cold70 | cold70 |
| رذاذ ماء لجلسات منعشة - 12 قطعة | mist | mist |
| جهاز ضباب نقي - 45 نزل | fogmachine | fogmachine |
| منقي الهواء 7 | Purifier7 | airpurifier7 |
| منقي الهواء برو | Purifier6 | airpurifier6 |
| منقي الهواء كلاسيك | Purifier4 | airpurifier4 |
| آلة تدوير الطعام | foodrecycling | recycling |
| مرطب هواء نقي | airhumidifier | airhumidifier |
| مضخة نقي | pumpnaqi | pumpnaqi |
| خلاط مجلى مزدوج | kitchdblefaucet | kitchdblefaucet |
| صنبور فاخر مقاس وسط | luxmedfaucet | luxmedfaucet |
| صنبور فاخر كبير | luxlargefaucet | luxlargefaucet |
| فلتر شاور كربوني | carbonshowerfltr | carbonshowerfltr |
| فلتر شاور مضيئ | luminousshowerfltr | luminousshowerfltr |
| فلتر شاور ثلاث وضعيات | 3filtershower | 3fltrshower |
| حوض نقي المطور | basin | basin |
| سلفر كيو + برادة ذكية | fltrslvrqclrsmart | fltrslvrqclrsmart |
| سلفر كيو + أكسترا بلس | fltrslvrqclrextplus | fltrslvrqclrextplus |
| ركن القهوة + دفاية داخلية | coffecornernaqiheater | coffecornernaqiheater |
| بلاك اديشن + شكل مكينة كوفي | fltrblkqclrcoffe | fltrblkqclrcoffe |
| جهاز+شكل مكينة كوفي+ دفاية داخلية | fltrslvrqclrcoffenaqiheater | fltrslvrqclrcoffenaqiheater |
| سلفر كيو + برادة S | fltrslvrqclrs | fltrslvrqclrs |
| سلفر كيو + برادة طويلة H1 | fltrslvrqclrh1 | fltrslvrqclrh1 |
| ديجتال 75 + برادة ذكية | digital75clrsmart | digital75clrsmart |
| ديرتنا + زر امان | filterdrtnaclrsafe | ilterdrtnaclrsafe |
| آلة تدوير الطعام + منقي +6مراحل | Purifier6recycling | Purifier6recycling |
| آلة تدوير الطعام + منقي +4مراحل | Purifier4recycling | Purifier4recycling |
| سيلفر كيو + خلاط مزدوج | FltrslvrqKitchenmixer | FltrslvrqKitchenmixer |
| سيلفر كيو + خلاط مزدوج فاخر | FltrslvrqKitchenmixerprem | FltrslvrqKitchenmixerprem |
| سيلفر كيو + برادة زر امان مطور | FltrslvrqClrSafe | FltrslvrqClrSafe |
| سيلفر كيو + برادة شكل ماكنية قهوة | FltrslvrqClrcoffee | FltrslvrqClrcoffee |
| برادة G1 | CLRG1 | CLRG1 |
| برادة GS | CLRGS | CLRGS |
| شاور فاخر | FLTRSHOWERPREM | FLTRSHOWERPREM |
| غطاس نقي | submersible | submersible |
| جامبو + مضخة | jumbpump | jumbpump |
| برادة وصانعة ثلج | clrt1 | clrt1 |
| سكالا | Skala | Skala |
| عام | Generic | Generic |
| قدر نقي | cookpotN1 | cookpotN1 |
| عصارة نقي | squeezer | squeezer |
| خلاط نقي | BlenderNaqi | BlenderNaqi |
| خلاط نقي دجيتال | BlenderDigitalNaqi | BlenderDigitalNaqi |
| خلاط طهي | BlenderCooking | BlenderCooking |
| فرن نقي | Oven | Oven |
| صانعة سلاش | Sluchmaker | Sluchmaker |
| قطاع الاعمال | B2b | B2b |
| قلاية هوائية | AirfryerP1 | AirfryerP1 |
| حماصة توست | ToasterR1 | ToasterR1 |
| غلاية نقي ريترو | RetrokettleR1 | RetrokettleR1 |
| غلاية القهوة المقطرة | coffeekettleN1 | coffeekettleN1 |
| صانعة حبيبات الثلج P-1 | IceP1 | IceP1 |
| صانعه كرات الثلج L-1 | IceL1 | IceL1 |
| صانعة مكعبات الثلج L-2 | IceL2 | IceL2 |
| القهوة المقطرة+المطحنه | NaqiCoffeeBundle1 | NaqiCoffeeBundle1 |
| القهوة المقطرة+الحماصه+المطحنه | NaqiCoffeeBundle2 | NaqiCoffeeBundle2 |
| بكج الافطار | NaqiBreckfastBundle / BreakfastPackage | NaqiBreckfastBundle / BreakfastPackage |
| برادة OD1 | clrod1 | clrod1 |
| محطات التحلية المركزية | CentralDesalination | CentralDesalination |

> **مثال المستخدم مطابق تماماً:** `SNPC_Purifier7_arp_VDO_SA_2026Q2_V3` → Purifier7 = منقي الهواء 7، arp = Air Purifiers، ويجب أن يكون الرابط بـ `&prod_category=airpurifier7` تماماً.

---

## 2) دروس عامة مؤكدة من مراجعة الحسابات الفعلية (Cross-account patterns)

تمت هذه المراجعة على 3 حسابات Snapchat عبر **Native Tools** فقط (`snapchat_adaccounts_ad_account_id_campaigns_get`, `snapchat_campaigns_campaign_id_adsquads_get`, `snapchat_adsquads_ad_squad_id_ads_get`, `snapchat_campaigns_campaign_id_stats_report_report`, `snapchat_adaccounts_ad_account_id_stats_report_report`) — **بدون استخدام الأدوات العامة الموحّدة** (`list_campaigns` / `fetch_campaign`) — تنفيذاً للقاعدة رقم 1.

الحسابات:
| الحساب | Account ID | إجمالي الحملات | نشطة الآن |
|---|---|---|---|
| Snapchat Naqi Generic Products | `05d06f8d-cd4f-487e-a6b3-99d89e1b9930` | 104 | 9 |
| Snapchat Naqi Generic - Installation Products | `536c395d-f6bf-4dca-9b8a-1a5d9b72398e` | 11 | 3 (منها 1 فعلياً VALID) |
| Snapchat Naqi (الحساب الرئيسي/الأقدم، منذ 2021) | `f4d8e01a-34a2-4dde-ace3-6761f326f515` | 201 | 6 |

**عملة الحسابات الثلاثة: USD** (حتى مع استهداف السعودية جغرافياً) — مهم عند نسخ أرقام الميزانية.
**Pixel ID مشترك** لكل حساب، يتكرر في كل Ad Squad ضمنه: `5e83e6d8-26c0-4535-8d42-bb54f1e3ed15` (نفس الـ Pixel لحسابي Generic Products و Installation).

### الأنماط المتكررة في الإعدادات الناجحة:
1. **"منتج واحد = Ad Squad واحد"** — لا تُجمَّع منتجات متعددة داخل Ad Squad واحد أبداً. البنية القياسية: Campaign واحدة بهدف واحد ← عشرات الـ Ad Squads كل واحد لمنتج مختلف بنفس الاستهداف/الميزانية المبدئية.
2. **إستراتيجية "اختبار ثم توسيع" (Test-then-Scale):** تبدأ حملة ABO بميزانية يومية موحّدة صغيرة على كل Ad Squad (مثلاً 400 وحدة/يوم لكل منتج)، وبعد فترة تشغيل يتم:
   - إيقاف الـ Ad Squads الضعيفة (تصبح `PAUSED` / `INVALID_NOT_EFFECTIVE_ACTIVE`).
   - رفع الميزانية اليومية للفائزة عدة مرات (شوهد رفع من 400 إلى 700–5,000 وحدة/يوم) وتبقى `ACTIVE`/`VALID` لأسابيع أو أشهر.
   - **الإشارة العملية على "الفوز":** بقاء الـ Ad Squad نشطاً + ميزانية أعلى من البقية = تم اعتباره فائزاً من الفريق سابقاً.
3. **حملات "Always-On" طويلة العمر تُبنى ولا تُعاد من الصفر:** بعض الـ Ad Squads تعمل منذ عام أو أكثر بنفس الاسم (مثل `DLVRY_SNPC_COFFEENAQI` منذ 2025) — يُضاف لها Ad جديد بنسخة موسمية (Ramadan/Eid/Adha/شهر) كل موسم، وتُوقف Ads الموسم القديم، **بدون إنشاء Ad Squad أو Campaign جديدة**. هذا يحافظ على تاريخ التعلّم (Learning Phase) لخوارزمية Snapchat.
4. **Optimization Goal حسب الهدف:**
   - حملات المبيعات/الليدز (ABO, pacing_level=AD_SQUAD): `optimization_goal=PIXEL_PURCHASE`، `bid_strategy=LOWEST_COST_WITH_MAX_BID` مع `bid_micro` صريح (سقف مزايدة يدوي، غالباً 3–20 وحدة)، `conversion_window` عادة `SWIPE_7DAY` أو `SWIPE_28DAY_VIEW_1DAY`.
   - حملات الوعي (CBO, pacing_level=CAMPAIGN): `optimization_goal=IMPRESSIONS`، `bid_strategy=AUTO_BID` بدون bid_micro يدوي.
5. **الاستهداف الفائز = وطني واسع + Interest/Lookalike + Targeting Expansion مفعّل** (`enable_targeting_expansion:true` مع `interest_expansion_option` و `custom_audience_expansion_option` مفعّلين)، عمر 18–55 حسب المنتج. الاستهداف الجغرافي الضيق (مدينة واحدة فقط) **لم يثبت نفسه** — راجع القسم 5.
6. **الـ Placement غالباً غير محدد (`UNSUPPORTED` = تلقائي عبر كل أماكن Snapchat)** — لا تقييد يدوي على مواضع العرض في الحملات الناجحة المراجَعة.
7. **الـ Ads كلها `type: REMOTE_WEBPAGE, render_type: STATIC`** (Webview تقود لصفحة الموقع مباشرة عبر الرابط)، وليست Deep Link أو App.

---

## 3) قواعد التسمية المؤكدة فعلياً من الحسابات (Confirmed Live Naming Patterns)

| المستوى | الصيغة | مثال حقيقي من الحساب |
|---|---|---|
| **Campaign (منظّم/سنوي)** | `{Year}_{Country}_NAQI_{Channel}_{Medium}_{ObjectiveCode}_{Tag}` | `2026_SA_NAQI_SOC_SNPC_BR-AW_Installation_Awareness` |
| **Campaign (وسم حر لمبادرة)** | `{Medium}_{ProductLine or Tag}` | `SA_NAQI_SOC_SNPC_LEAD-GEN_PriceCampaign2026`, `2026_NAQI_SOC_Snpc_CONV_PUR_AlwaysOn_shahin` |
| **Ad Squad (داخل CBO/Awareness — منتج واحد)** | `{Medium}_{ProductCode}_{ProductCategoryCode}_{AdFormatCode}_{Country}_{CampaignTag}` | `SNPC_submersible_scd_VDO_SA_Installation_Awareness` |
| **Ad Squad (داخل ABO/Testing — منتج واحد)** | `{Medium}_{ProductCode}_{ProductCategoryCode}_{CampaignTag}` | `SNPC_Fltrjmb_wtrflt_PriceCampaign2026` |
| **Ad Squad (Always-On/Delivery)** | `DLVRY_{Medium}_{PRODUCT_NAME}` | `DLVRY_SNPC_COFFEENAQI`, `DLVRY_SNPC_ALL_PURIFIERS` |
| **Ad Squad (Evergreen Interest testing)** | `{Medium}_INT_{ProductCategoryCode}_{CreativeAngle}` | `SNPC_INT_wtrflt_NewDesigns`, `SNPC_INT_wtrflt_ZaidVideos` |
| **Ad (الصيغة القياسية المعتمدة — مطابقة لمثال المستخدم)** | `{Medium}_{ProductCode}_{ProductCategoryCode}_{AdFormatCode}_{Country}_{Year}Q{Quarter}_V{n}` | ` SNPC_coffeenaqi_cfm_VDO_SA_2026Q2_V1` … `V6` (موجودة فعلياً وتعمل الآن) |
| **Ad (نسخة موسمية مقبولة)** | نفس الصيغة لكن الوسم الزمني يصبح اسم الموسم/الشهر بدل `{Year}Q{Quarter}` | `SNPC_coffeenaqi_cfm_VDO_SA_adha2026_V4`, `SNPC_coffeenaqi_cfm_VDO_SA_ramadan2026_V3`, `SNPC_coffeenaqi_cfm_VDO_SA_Jun2026_V1` |

**القاعدة الصارمة (لا استثناء):** اسم الـ Ad أعلاه = قيمة `source` = قيمة `utm_source` = قيمة `utm_campaign` في الرابط حرفياً، و `prod_category` في الرابط = القيمة من عمود `prod_category (URL)` في الشيت لنفس المنتج (وليس Product Code).
مثال تحقق فعلي: Ad اسمه `SNPC_coffeenaqi_cfm_VDO_SA_2026Q2_V1` → المنتج "قهوة نقي المقطرة" → `prod_category=coffeenaqi` (من جدول القسم 1.2)، وليس `cfm` (كود الفئة) ولا أي قيمة أخرى.

---

## 4) حالات ناجحة موثّقة (Documented Success Cases)

### Case 1 — DLVRY_SNPC_COFFEENAQI (Always-On Delivery, قهوة نقي المقطرة)
- **الحساب/المنصة:** Snapchat Naqi Generic Products (`05d06f8d-…`)
- **المنتج/السوق:** قهوة نقي المقطرة (coffeenaqi) — السعودية
- **هدف الحملة:** SALES → Lead-Gen/Purchase توصيل (Campaign: `2026_NAQI_SOC_Snpc_CONV_LEAD-GEN_AlwaysOn_Delevery`, نشطة منذ 2025-01-08)
- **الهيكلة:** Campaign واحدة دائمة (Always-On) تحوي ~146 Ad Squad تراكمت منذ أكثر من عام (منتج واحد لكل Ad Squad)؛ الناجي والنشط منها الآن Ad Squad واحد باسم `DLVRY_SNPC_COFFEENAQI` يحوي 44 Ad تراكمياً، منها 10 نشطة الآن بالتوازي (اختبار إبداعي مستمر داخل نفس الـ Ad Squad).
- **الاستهداف:** SA وطنية، عمر 20–50، بدون تضييق جغرافي، Targeting Expansion مفعّل.
- **Placement:** تلقائي (كل مواضع Snapchat).
- **Optimization Event:** `PIXEL_PURCHASE` على Pixel `5e83e6d8-…`
- **Budget/Bidding:** `LOWEST_COST_WITH_MAX_BID`، `bid_micro=3,000,000` (سقف ~3 وحدات)، `daily_budget_micro=5,000,000,000` (~5,000 وحدة/يوم) — **أعلى ميزانية بين كل منتجات DLVRY** في هذه الحملة → إشارة على أنه المنتج الأقوى تحويلاً بالتوصيل. `conversion_window=SWIPE_7DAY`.
- **Creative/Copy:** فيديو REMOTE_WEBPAGE بصيغ متعددة (VDO أساسي + IMG بديل)، نسخ موسمية متكررة كل ربع/موسم (Ramadan, Eid, Adha, يونيو…)، مثال أسماء فعلية: `SNPC_coffeenaqi_cfm_VDO_SA_2026Q2_V1..V6`, `SNPC_coffeenaqi_cfm_VDO_SA_adha2026_V1..V5`, `SNPC_coffeenaqi_cfm_VDO_SA_Jun2026_V1..V4`.
- **Naming/URLs/UTMs:** يطابق القاعدة القياسية في القسم 3 (Medium_ProductCode_CategoryCode_Format_Country_Season/Quarter_V#). `prod_category=coffeenaqi`.
- **فترة التشغيل:** مستمرة منذ 2025-05 تقريباً (أول Ad) وحتى الآن (2026-08) بدون توقف — أكثر من سنة كاملة.
- **النتيجة الأساسية:** الإنفاق الكلي للحملة `AlwaysOn_Delevery` منذ 2025-01 وحتى الآن ≈ **1,478,627 USD** بـ **657.6M** ظهور (Impressions) — أعلى إنفاق واستمرارية بين كل حملات الحساب، وهذا Ad Squad أعلى ميزانية داخلها.
- **وش نجح وليش:** الاستمرارية (عدم إعادة بناء الـ Ad Squad)، تنويع الإبداع الموسمي بدل تكرار نفس الفيديو، واستهداف وطني واسع بدون تضييق جغرافي أو ديموغرافي زائد.
- **يمكن تكراره/تطويره:** استخدم نفس البنية (Ad Squad دائم باسم `DLVRY_SNPC_{Product}` + Ads موسمية جديدة) لأي منتج جديد يُراد إطلاقه بنموذج Always-On، بدل حملة جديدة كل مرة.

### Case 2 — SNPC_Fltrjmb_wtrflt_PriceCampaign2026 (فلتر جامبو — فائز من اختبار ABO)
- **الحساب/المنصة:** Snapchat Naqi Generic Products
- **المنتج/السوق:** فلتر جامبو (Fltrjmb/Jumbofilter) — السعودية
- **هدف الحملة:** SALES (Campaign: `SA_NAQI_SOC_SNPC_LEAD-GEN_PriceCampaign2026`, بدأت 2026-06-25)
- **الهيكلة:** حملة ABO بها 12 Ad Squad (منتج واحد لكل واحد: Clrm, Clrd, CLRGS, jumbpump, pumpnaqi, Fltrblk, clrod1, Clre, clrt1, proclrpls, Clru1, **Fltrjmb**). بعد أسابيع التشغيل، 6 منها نجت (`ACTIVE`/`VALID`) و6 أوقفت.
- **الاستهداف:** SA، عمر 18+، Smart Targeting Expansion (`auto_expansion_type: SMART_TARGETING`) مفعّل.
- **Optimization Event:** `PIXEL_PURCHASE`، `conversion_window=SWIPE_7DAY`.
- **Budget/Bidding:** `LOWEST_COST_WITH_MAX_BID`، بدأ الجميع بـ`bid_micro` قريب (7–15.5M) و`daily_budget_micro` موحّد تقريباً ثم تفاوت بعد التوسيع — **Fltrjmb انتهى بأعلى ميزانية يومية: 1,400,000,000 (~1,400 وحدة/يوم)**، يليه jumbpump وclrod1 (1,300)، Clru1 (1,100)، Clre (700).
- **فترة التشغيل:** من 2026-07-09 (بعد أسبوعين اختبار) وحتى الآن، مستمرة.
- **النتيجة الأساسية:** إنفاق الحملة كاملة ≈ **38,118 USD** بـ **25.66M** ظهور خلال ~6 أسابيع — من أعلى معدلات الإنفاق النشط حالياً في الحساب.
- **وش نجح وليش:** نموذج "امنح كل منتج فرصة متساوية بميزانية صغيرة، ثم اقطع الميزانية عن الأضعف وضخّها في الأفضل" — تم تكراره بنجاح عدة مرات في هذا الحساب (نفس النمط في Installation و AlwaysOn_Delevery).
- **يمكن تكراره:** ابدأ أي دفعة منتجات جديدة (Launch جماعي) بنفس القالب: Ad Squad واحد/منتج، ميزانية ابتدائية موحّدة صغيرة (300–500 وحدة/يوم)، مراجعة أسبوعية، ورفع الميزانية 2-3x للفائز فقط.

### Case 3 — Installation_Awareness (حملة وعي CBO لكل منتجات التركيب)
- **الحساب/المنصة:** Snapchat Naqi Generic - Installation Products (`536c395d-…`)
- **المنتج/السوق:** منتجات متعددة (فلتر سلفر كيو، برادة GS، فلتر ديرتنا، جامبو، فلتر بلاك اديشن، برادة OD1، سوبر 200، مِست…) — السعودية
- **هدف الحملة:** AWARENESS_AND_ENGAGEMENT (Campaign: `2026_SA_NAQI_SOC_SNPC_BR-AW_Installation_Awareness`, بدأت 2026-07-27، **CBO على مستوى الحملة**)
- **الهيكلة:** 8 Ad Squads، منتج واحد لكل واحد، جميعها `ACTIVE`/`VALID` بالتوازي (لا يوجد فائز/خاسر بعد — حملة حديثة).
- **الاستهداف:** SA، عمر 20+، Interest + Custom Audience Expansion مفعّلين.
- **Optimization Event:** `IMPRESSIONS` (مشترك على مستوى الحملة عبر `campaign_budget_optimization_shared_properties`)، bidding: `AUTO_BID`.
- **Budget:** Lifetime Budget مشترك 425.99 USD لكل الحملة (توزيع تلقائي بين الـ Ad Squads عبر CBO)، تنتهي 2026-08-10.
- **Naming:** `SNPC_{ProductCode}_{CategoryCode}_VDO_SA_Installation_Awareness` لكل Ad Squad — كلها فيديو (VDO).
- **فترة التشغيل:** 2026-07-27 → 2026-08-10 (~2 أسابيع، Lifetime Budget قصيرة المدى).
- **النتيجة:** لم تكتمل الفترة وقت هذه المراجعة — **يُحدَّث هذا القسم بعد انتهاء الحملة بالنتائج ونِسَب الظهور/التكلفة لكل منتج.**
- **الدرس التشغيلي:** هذا نموذج "دفعة وعي جماعية بميزانية سقفية عمرية (Lifetime Budget) + CBO" — بديل مختلف عن نموذج ABO في Case 2. مفيد لإطلاقات الوعي قصيرة المدى (موسم/عرض)، وليس لحملات المبيعات المستمرة.

### Case 4 — 2025_SA_NAQI_SOC_SNPC_CONV_ABO_TOPPERFOMINGCAMPAIGN (استهداف Interest دائم — منقيات المياه)
- **الحساب/المنصة:** Snapchat Naqi (الحساب الرئيسي/الأقدم) — الحملة اسمها الحرفي يتضمن "TOPPERFOMINGCAMPAIGN" (وسمها الفريق بهذا الاسم صريحاً كإشارة نجاح).
- **المنتج/السوق:** فئة Water Filters (wtrflt) عامة — السعودية
- **هدف الحملة:** BRAND_AWARENESS (لكن الـ Ad Squads كلها مُحسَّنة فعلياً على `PIXEL_PURCHASE` — استخدام عملي لهدف مبيعات تحت غلاف حملة Awareness)، بدأت 2025-10-16، **لا تزال شغالة بعد نحو 10 أشهر متواصلة**.
- **الهيكلة:** 6 Ad Squads بنمط `SNPC_INT_wtrflt_{CreativeAngle}` (NewIdeas, AllDesigns, Videos, NewDesigns, VideoTest, ZaidVideos) — كل واحد يمثل زاوية إبداعية مختلفة على نفس الفئة والاستهداف، وليس منتجاً مختلفاً.
- **الاستهداف:** SA، عمر 20–55، أجهزة WEB/iOS/Android، Interest + Custom Audience Expansion.
- **Optimization Event:** `PIXEL_PURCHASE`، `LOWEST_COST_WITH_MAX_BID` بسقف مزايدة 9M (~9 وحدات)، `conversion_window=SWIPE_28DAY_VIEW_1DAY`.
- **Budget:** 3 من 6 Ad Squads نجت وبقيت نشطة برفع ميزانية: NewDesigns (1,000/يوم)، ZaidVideos (1,200/يوم)، VideoTest (600/يوم). الباقي (NewIdeas, AllDesigns, Videos) أوقفت.
- **فترة التشغيل:** 2025-10-16 → مستمرة حتى اليوم (2026-08-05) — **أطول حملة نشطة تمت مراجعتها في هذا الجرد.**
- **وش نجح وليش:** تسمية Ad Squad بزاوية الإبداع (بدل المنتج) عند استهداف فئة كاملة بدل منتج واحد؛ الاستمرارية طويلة المدى مع تدوير الإبداع فقط (نفس منطق Case 1)؛ "ZaidVideos" تشير لاستخدام محتوى صانع/فريق معيّن نجح بشكل خاص — يُنصح بالتحقق من نوع هذا المحتوى (احتمال UGC أو Influencer) وتوسيعه لمنتجات أخرى.
- **يمكن تطويره:** طبّق نفس الاسم/البنية (`SNPC_INT_{CategoryCode}_{CreativeAngle}`) على فئات أخرى ذات طلب مستمر (مثل Air Purifiers أو Coolers) كحملة Evergreen مستقلة عن حملات الإطلاقات الموسمية.

### Case 5 — TikTok Naqi Silver: تأكيد المنتجات الفائزة عبر منصتين (Cross-Platform Confirmation)
- **المصدر:** تقرير Spend-by-Ad-by-Day مرفوع من المستخدم (`TikTokAds_abdulqader_report_TikTok_Naqi_SIlver`, الفترة 2026-07-31 → 2026-08-06، 7 أيام، حساب TikTok Naqi Silver `6804327175068581893`). **لم يُسحَب عبر Native TikTok API مباشرة** (اتصال Whathead كان غير مُفوَّض وقت هذه المراجعة) — بل عبر تحليل ملف تقرير جاهز رفعه المستخدم.
- **الملاحظة الأهم:** التسمية على TikTok تطابق حرفياً نفس قالب Snapchat مع تبديل كود المنصة فقط: `TKK_{ProductCode}_{ProductCategoryCode}_VDO_SA_{SeasonTag}_V{n}` — مثال: `TKK_Fltrslvrq_wtrflt_VDO_SA_Jun2026_V17`. هذا يؤكد أن قالب التسمية في القسم 3 **موحّد عبر المنصات** (SNPC/TKK/…)، وليس خاصاً بسناب شات فقط.
- **توزيع الإنفاق الأسبوعي (63 إعلان نشط، إجمالي ≈ 5,772 USD/أسبوع):**
  | Product Code | الإنفاق (USD) | % من الإجمالي |
  |---|---|---|
  | **Fltrslvrq** (فلتر سلفر كيو) | 4,760.06 | ~82% |
  | Fltrblk (بلاك اديشن) | 336.87 | ~6% |
  | Clru1 (برادة U1) | 299.15 | ~5% |
  | CLRGS (برادة GS) | 199.72 | ~3.5% |
  | Fltrjmb (فلتر جامبو) | 127.39 | ~2% |
  | jumbpump (جامبو+مضخة) | 49.07 | ~1% |
- **أهم إعلانين منفردين:** `TKK_Fltrslvrq_wtrflt_VDO_SA_Jun2026_V17` (1,284 USD) و `TKK_Fltrslvrq_wtrflt_VDO_SA_Jun2026_V27` (1,095 USD) — من إجمالي أكثر من 30 نسخة فيديو (V1…V34) تحت وسم `Jun2026` لنفس المنتج، بجانب نسخ موازية تحت وسم `Summer2026`.
- **التقاطع الحاسم مع Snapchat:** **Fltrslvrq, Clru1, CLRGS, Fltrjmb, jumbpump** هي بالضبط نفس المنتجات التي ظهرت كفائزة/مُوسَّعة الميزانية في Case 2 (PriceCampaign2026 على Snapchat). أي أن هذه المجموعة من المنتجات أثبتت نفسها **عبر منصتين مختلفتين بشكل مستقل** — أقوى إشارة نجاح في هذا الملف حتى الآن.
- **وش نجح وليش:** (أ) نفس قالب التسمية يُستخدم بلا تعديل بين المنصات، فقط كود Medium يتغيّر — يسهّل النسخ بين الحسابات. (ب) اختبار عدد كبير من نسخ الفيديو (V1-V34) لنفس المنتج تحت نفس الوسم الزمني، مع ترك الإنفاق يتوزع طبيعياً حتى تتضح النسخ الأقوى (V17, V27) بدل قصر الاختبار على نسخة أو نسختين.
- **يمكن تكراره:** عند إطلاق منتج جديد على منصة جديدة، ابدأ بمنتجات هذه القائمة (Fltrslvrq أولاً) بدل تجربة عشوائية — نجاحها متكرر ومستقل عن المنصة.
- ⚠️ **حدود هذا الرصد:** الرقم هو Spend فقط من تقرير جاهز، بدون Purchases/CPA/ROAS، وبدون معرفة الـ Campaign/Ad Group الأصلي أو الاستهداف/الميزانية (الملف كان "Ad name × Day × Spend" فقط). يُستكمل لاحقاً بسحب مباشر عبر Native TikTok Tools (`tiktok_campaign_get`, `tiktok_report_*`) بعد إعادة تفويض Whathead، لإضافة الاستهداف والـ CPA الحقيقي كما فُعل مع Snapchat.

---

## 5) ما لم يعمل / دروس سلبية (What Didn't Work — لتجنّب تكرارها بدون سبب)

### الاستهداف الجغرافي الضيق (GEO_RYD) لم يثبت نفسه
- لوحظت جولة اختبار كاملة (`2026_SA_NAQI_SOC_SNPC_CONV_ABO_ADHA2026`, حساب Installation) بها **23 Ad Squad** بصيغة `SNPC_GEO_RYD_{Category}_{PRODUCT}` — تستهدف مدينة الرياض فقط، عمر 18+، بميزانية موحّدة 400 وحدة/يوم و`bid_strategy=TARGET_COST`.
- **النتيجة:** كل الـ 23 توقفت (`INVALID_NOT_ACTIVE` / `INVALID_NOT_EFFECTIVE_ACTIVE`) ولا يوجد ناجٍ واحد نشط الآن من هذه الدفعة بالكامل.
- **الاستنتاج:** التضييق الجغرافي لمدينة واحدة + TARGET_COST bidding لم يكن النمط الفائز في هذا الحساب — الأنماط التي نجحت وبقيت نشطة (Cases 1-4 أعلاه) كانت دوماً استهداف **وطني (SA)** واسع مع Interest/Lookalike و Targeting Expansion، وbidding من نوع `LOWEST_COST_WITH_MAX_BID` أو `AUTO_BID` (نادراً `TARGET_COST`).
- **توصية:** لا تُستخدم `TARGET_COST` + تضييق مدينة واحدة كنقطة انطلاق افتراضية لمنتج جديد؛ ابدأ وطنياً واسعاً كما في Case 2.

---

## 6) الفجوات وحدود هذه المراجعة (Coverage & Limitations) — مهم للشفافية

- ✅ تمت المراجعة بالكامل عبر **Native Snapchat Tools** فقط (بدون أدوات عامة موحّدة)، تنفيذاً للقاعدة رقم 1.
- ✅ Naqi Generic - Installation Products: تمت مراجعة **كل الحملات (11)** على مستوى Campaign، وتفصيل كامل (Ad Squads) لأهم 2 منها.
- ✅ Naqi Generic Products: تمت مراجعة **كل الـ 9 حملات النشطة** على مستوى الإنفاق/الظهور، وتفصيل Ad Squad + Ad لعينة منها (AlwaysOn_Delevery, PriceCampaign2026).
- ⚠️ Naqi (الحساب الرئيسي): يحوي **201 حملة** تاريخية منذ 2021 — تمت مراجعة **الـ 6 النشطة حالياً بالتفصيل فقط** (خصوصاً TOPPERFOMINGCAMPAIGN)، ولم تُراجَع الحملات المتوقفة القديمة (~195) فردياً؛ أُخذت عينة فقط.
- ⚠️ **لم يتم استخراج أرقام دقيقة لـ Purchases/CPA/ROAS لكل حملة** بسبب Rate Limiting على Snapchat Async Reports API أثناء هذه الجلسة (طلبات `stats_report` كانت تتعطل بشكل متكرر). الاعتماد الحالي على:
  1. حالة التشغيل (`ACTIVE`/`VALID`) كإشارة "لا يزال يعمل" (أحد معياري طلب المستخدم مباشرة).
  2. توزيع/رفع الميزانية بين الـ Ad Squads كإشارة على "الفائز" (ميزانية أعلى + بقاء نشط = اعتُبر فائزاً من الفريق سابقاً).
  3. الإنفاق/الظهور الكلي للحملة كمؤشر حجم واستثمار.
  **لا تعتبر هذا القسم نهائياً** — يُنصح بجولة تالية مخصصة لسحب `conversion_purchases`, `conversion_purchases_value`, `swipes` بدقة لكل حملة نشطة عبر `stats_report` (مع إعادة تزويد نفس شكل الطلب عند الـ polling لتفادي القيم المبتورة)، وتحديث Cases 1-4 بأرقام CPA/ROAS الحقيقية.
- ⚠️ **TikTok:** تمت إضافة Case 5 (Naqi Silver) بالاعتماد على **تقرير Excel جاهز رفعه المستخدم** (Spend فقط، أسبوع واحد)، وليس عبر Native TikTok Tools مباشرة — لأن اتصال Whathead كان يحتاج إعادة تفويض وقت المراجعة. لم تتم مراجعة حسابي TikTok الآخرين (TikTok Naqi Generic, Naqi Generic Products) ولا استهداف/بنية Ad Group/Campaign الحقيقية على TikTok بعد.
- ⚠️ لم تتم مراجعة Meta حتى الآن. يُستكمل تدريجياً كل ما توفّر اتصال Native بالمنصة.

---

## 7) قائمة تحقق قبل إنشاء أي Campaign / Ad Set / Ad جديد

- [ ] راجع هذا الملف (Memory.md) — هل توجد Case مشابهة لنفس المنتج/المنصة/الهدف؟ ابدأ منها.
- [ ] راجع الحملات **النشطة حالياً** على الحساب المستهدف عبر Native Tools قبل إنشاء أي شيء جديد.
- [ ] افتح `Naming Tool.xlsx` مباشرة واستخرج: Product Code، Product Category Code، prod_category — **لا تُكتب من الذاكرة أبداً**.
- [ ] تأكد أن اسم الـ Ad = `source` = `utm_source` = `utm_campaign` حرفياً بدون أي فرق.
- [ ] تأكد أن `prod_category` في الرابط مطابق تماماً لعمود `prod_category (URL)` لنفس المنتج في الشيت.
- [ ] فحص الرابط كاملاً + التسمية قبل نشر أي إعلان مباشرة.
- [ ] بعد فترة تشغيل كافية: عُد ووثّق النتيجة في القسم 4 أعلاه (نجحت أو فشلت) — القسم 4 يكبر مع كل حملة جديدة.
