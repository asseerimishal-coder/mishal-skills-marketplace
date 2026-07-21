# mishal company — مكتبة المهارات (Skills Marketplace)

سوق مهارات موحّد لشركة **mishal company**، منظّم في **7 بلقنات** حسب الأقسام، بإجمالي **175 مهارة** جاهزة للتركيب في Claude / Cowork.

## الهيكل التنظيمي

```
mishal-skills-marketplace/
├── .claude-plugin/
│   └── marketplace.json        ← ملف السوق الرئيسي (يعرّف الـ7 بلقنات)
├── developers/                 ← بلقن المطورين (38 مهارة)
│   ├── .claude-plugin/plugin.json
│   └── skills/ … (كل مهارة مجلد فيه SKILL.md)
├── designers/                  ← بلقن المصممين (25 مهارة)
├── marketing/                  ← بلقن التسويق (47 مهارة)
├── social-media/               ← بلقن السوشال ميديا (17 مهارة)
├── finance/                    ← بلقن المالية (8 مهارات)
├── small-business/             ← بلقن إدارة المشاريع الصغيرة (31 مهارة)
└── legal/                      ← بلقن القسم القانوني (9 مهارات)
```

## البلقنات

| البلقن | القسم | عدد المهارات |
|--------|-------|--------------|
| developers | المطورين | 38 |
| designers | المصممين | 25 |
| marketing | التسويق | 47 |
| social-media | السوشال ميديا | 17 |
| finance | المالية | 8 |
| small-business | إدارة المشاريع الصغيرة | 31 |
| legal | القسم القانوني | 9 |

## طريقة التركيب

الطريقة الأنسب: ارفع هذا المجلد كمستودع على GitHub، ثم في Claude Code:

```
/plugin marketplace add <your-org>/mishal-skills-marketplace
/plugin install developers@mishal-skills
```

كل موظف يركّب بلقن قسمه فقط. التحديث لاحقاً من مكان واحد (المستودع)، والجميع يستفيد.

## التحديث

عدّل المهارات في المستودع → ارفع (push) → الفريق يعمل `/plugin update`. الهوية والإصدارات تُدار مركزياً من ملفات `plugin.json` و `marketplace.json`.

> لا تنسى ذكر الله، والصلاة على النبي ﷺ
