<div align="center">

# 🛡️ Pro Engineering & Security Skills

**حزمة سكلز تخلّي أي مساعد ذكاء اصطناعي يبرمج كمهندس خبير ويراجع كمختص أمن**

![Version](https://img.shields.io/badge/version-2.0-blue)
![Skills](https://img.shields.io/badge/skills-26-success)
![Format](https://img.shields.io/badge/format-Agent%20Skills%20(SKILL.md)-purple)
![Platforms](https://img.shields.io/badge/works%20with-Claude%20%7C%20ChatGPT%20%7C%20Codex%20%7C%20Cursor%20%7C%20Copilot%20%7C%20Gemini-orange)

[العربية](#-نبذة) · [English](#-english)

</div>

---

<div dir="rtl">

## 📌 نبذة

لما تطلب من الذكاء الاصطناعي يكتب كود، غالباً يعطيك كود "يشتغل" لكنه ناقص: ما فيه اختبارات، ما يتحقق من الصلاحيات، يخترع مكتبات ما لها وجود، أو يقول لك "الاختبارات نجحت" وهو ما شغّلها أصلاً.

هالحزمة تحل هالمشكلة. هي مجموعة **26 سكل** (ملفات تعليمات منظمة بصيغة `SKILL.md` المفتوحة) تركّبها مرة وحدة، وبعدها المساعد يلتزم تلقائياً بمعايير البرمجة الاحترافية ومعايير أمن التطبيقات في كل مهمة.

- ✅ تشتغل على **Claude** و **ChatGPT** و **Codex** و **Cursor** و **GitHub Copilot** و **Gemini**
- ✅ مستقلة عن لغة البرمجة والإطار (Python، JavaScript/TypeScript، Java، Go، C#، PHP، …)
- ✅ تدعم **العربي** في الردود، و **RTL** في الواجهات
- ✅ فيها نسخ جاهزة لكل منصة، ما تحتاج تعدّل شي

---

## ✨ وش يتغير بعد التركيب؟

| بدون الحزمة | مع الحزمة |
|---|---|
| كود بدون اختبارات | كل تغيير معه اختبارات، منها حالات سلبية وحالات حدّية |
| "الاختبارات نجحت" بدون دليل | يقول بوضوح هل شغّل الاختبارات أو **"not run"** ويعطيك الأوامر |
| يخترع مكتبات ودوال | ممنوع يخترع، وإذا ما هو متأكد يقول ويوضح كيف تتحقق |
| يجيب السجل بالـ id بس | يقيّد الاستعلام بالمستخدم والمستأجر (tenant) ويرفض الوصول افتراضياً |
| يحط الأسرار في الكود | يستخدم مدير الأسرار، وما يحط أسرار في الكود أو السجلات أو البرومبت |
| يعيد كتابة الملف كامل | يسوي أصغر تغيير صحيح ويلتزم بأسلوب مشروعك |
| رد عشوائي الشكل | ملخص ← كود ← طريقة التشغيل ← حالة التحقق ← المخاطر |

---

## 📚 محتوى الحزمة

### 🧭 السكل الأساسي (يشتغل دائماً)

| السكل | الوصف |
|---|---|
| `eng-core-standards` | طريقة الفهم والتخطيط والتنفيذ والتحقق والتقرير، تعريف "المهمة مكتملة"، قواعد الصدق، وجدول يوجّه لباقي السكلز |

### 💻 سكلز البرمجة (14)

| السكل | يغطي |
|---|---|
| `eng-code-quality` | التسمية، حجم الدوال، التعقيد، معالجة الأخطاء، معايير كل لغة |
| `eng-architecture` | تقسيم الوحدات، الطبقات، الأنماط، الأنظمة الموزعة، قرارات المعمارية (ADR) |
| `eng-testing` | هرم الاختبارات، الحالات الحدّية، الاختبارات المتقطعة، Property-based و Mutation testing |
| `eng-code-review` | قائمة مراجعة شاملة، تصنيف الملاحظات حسب الخطورة، صيغة الملاحظة |
| `eng-debugging` | منهجية علمية لتتبع الخطأ، أسباب شائعة، التعامل مع الحوادث |
| `eng-performance` | القياس قبل التحسين، N+1، الفهارس، الكاش، Core Web Vitals |
| `eng-api-design` | REST و GraphQL و gRPC، أكواد الحالة، صيغة الأخطاء RFC 9457، الترقيم، الإصدارات |
| `eng-database` | تصميم الجداول، القيود، الفهارس، المعاملات، الترحيل بدون توقف |
| `eng-frontend` | المكونات، إدارة الحالة، إمكانية الوصول WCAG 2.2، **العربي و RTL**، الأداء |
| `eng-observability` | معالجة الأخطاء، السجلات المنظمة، المقاييس، التتبع، التنبيهات |
| `eng-git-workflow` | الفروع، Conventional Commits، وصف الـ PR، الإصدارات، إصلاح أخطاء Git |
| `eng-documentation` | README، التوثيق المرجعي، ADR، Runbooks، التوثيق ثنائي اللغة |
| `eng-refactoring` | إعادة الهيكلة الآمنة، الكود القديم، Strangler Fig، ترقية الأطر |
| `eng-devops` | CI/CD، Docker، Kubernetes، البنية ككود (IaC)، استراتيجيات النشر |

### 🔐 سكلز الأمن (11)

| السكل | يغطي |
|---|---|
| `sec-authentication` | تسجيل الدخول، OIDC، كلمات المرور، MFA و Passkeys، الجلسات، JWT |
| `sec-authorization` | الصلاحيات، عزل المستأجرين، IDOR و BOLA، الرفض الافتراضي |
| `sec-api-security` | OWASP API Security Top 10، CORS، مفاتيح API، Webhooks |
| `sec-frontend-security` | XSS، سياسة CSP والهيدرات الأمنية، تخزين التوكنات، الأسرار في الواجهة |
| `sec-backend-security` | الحقن بأنواعه، SSRF، رفع الملفات، فك التسلسل، التشفير |
| `sec-data-protection` | تصنيف البيانات، التشفير، الاحتفاظ والحذف، **نظام حماية البيانات الشخصية PDPL**، إدارة الأسرار |
| `sec-audit-logging` | أحداث التدقيق الإلزامية، صيغة السجل، الخصوصية، التنبيه على النشاط المشبوه |
| `sec-security-review` | مراجعة أمنية منظمة، تصنيف الخطورة، قالب التقرير، قرار الحجب أو الموافقة |
| `sec-threat-modeling` | نمذجة التهديدات بطريقة STRIDE، حالات إساءة الاستخدام، ربط الحلول بالاختبارات |
| `sec-supply-chain` | التحقق من المكتبات، الحزم الوهمية اللي يخترعها الذكاء الاصطناعي، SBOM، تأمين CI |
| `sec-ai-llm-security` | OWASP Top 10 لتطبيقات LLM، حقن البرومبت، صلاحيات الوكلاء، RAG |

---

## 🚀 التركيب

كل النسخ الجاهزة موجودة في مجلد [`dist/`](dist/). نفس المحتوى، بس كل مجلد مغلّف حسب المنصة.

### Claude.ai أو تطبيق Claude

1. حمّل ملفات الـ zip من [`dist/skill-zips/`](dist/skill-zips/)
2. روح **Settings ← Capabilities ← Skills ← Upload skill**
3. ارفع كل ملف zip، وابدأ بـ `eng-core-standards.zip`

> تحتاج خطة فيها ميزة Skills وتنفيذ الكود مفعّل.

### ChatGPT

| الحالة | الطريقة |
|---|---|
| عندك ميزة **Skills** | Skills ← Create ← Upload from your computer، وارفع نفس ملفات الـ zip |
| تبي **Custom GPT** | Create GPT ← Configure، وانسخ [`dist/chat-projects/INSTRUCTIONS.txt`](dist/chat-projects/INSTRUCTIONS.txt) في خانة Instructions، وارفع الأربع ملفات من [`knowledge/`](dist/chat-projects/knowledge/) |
| تستخدم **Projects** | تعليمات المشروع هي `INSTRUCTIONS.txt`، وملفات المشروع هي محتوى `knowledge/` |
| تبي تطبقها على **كل محادثاتك** | انسخ [`SHORT_INSTRUCTIONS.txt`](dist/single-file/SHORT_INSTRUCTIONS.txt) في Settings ← Personalization ← Custom instructions |

### أدوات البرمجة (تنسخها لجذر مشروعك)

| الأداة | المجلد | وش تنسخ |
|---|---|---|
| Claude Code | [`dist/claude-code/`](dist/claude-code/) | `.claude/` و `CLAUDE.md` و `policy/` |
| OpenAI Codex | [`dist/codex-agents/`](dist/codex-agents/) | `.agents/` و `AGENTS.md` و `policy/` |
| Cursor | [`dist/cursor/`](dist/cursor/) | `.cursor/rules/` و `AGENTS.md` و `policy/` |
| GitHub Copilot | [`dist/copilot/`](dist/copilot/) | `.github/copilot-instructions.md` و `docs/ai-skills/` و `policy/` |
| Gemini CLI | [`dist/gemini-cli/`](dist/gemini-cli/) | `GEMINI.md` و `docs/ai-skills/` و `policy/` |

مثال لـ Claude Code:

</div>

```bash
git clone https://github.com/<your-org>/<this-repo>.git
cp -r <this-repo>/dist/claude-code/. /path/to/your-project/
```

<div dir="rtl">

> بعد النسخ، افتح ملف التعليمات (`CLAUDE.md` أو `AGENTS.md` أو غيره) وعبّئ قسم **Project specifics**: أوامر البناء والاختبار، مزود الهوية، ومسؤول الأمن.

### أي محادثة بدون إعداد

ارفق ملف [`dist/single-file/ALL_SKILLS.md`](dist/single-file/ALL_SKILLS.md) واكتب:

> التزم بهذي المعايير في هالمحادثة.

---

## 🧪 تأكد إن التركيب اشتغل

اكتب للمساعد:

> اكتب endpoint يرجّع فاتورة حسب الـ id في نظام متعدد المستأجرين

إذا التركيب صحيح، بيطلع لك:

- استعلام مقيّد بالـ `tenant_id` جاي من الجلسة، مو من الطلب
- رد 401 لغير المسجّل، و 404 لفاتورة تابعة لمستأجر ثاني
- تحقق من المدخلات
- اختبارات سلبية، منها اختبار الوصول لبيانات مستأجر ثاني
- سطر يوضح هل الاختبارات اشتغلت فعلاً أو "not run"

---

## 🗂️ هيكل المستودع

</div>

```text
.
├── skills/                      # مصدر السكلز (عدّل هنا)
│   ├── eng-core-standards/      #   السكل الأساسي
│   ├── eng-*/                   #   14 سكل برمجة
│   └── sec-*/                   #   11 سكل أمن
├── policy/
│   ├── ENGINEERING_STANDARDS.md # ENG-001 … ENG-011
│   ├── SECURITY_POLICY.md       # SEC-001 … SEC-014
│   ├── CONTROL_MATRIX.csv       # الضوابط، طريقة التحقق، المالك، الحالة
│   └── QUALITY_GATES.md         # بوابات الجودة المطلوبة
├── templates/                   # قوالب تعليمات المنصات (Custom GPT، التعليمات القصيرة، …)
├── ci/PR_CHECKLIST.md           # قائمة تحقق طلبات الدمج
├── examples/                    # مثال مرجعي للصلاحيات + قالب ربط المشروع
├── tests/                       # اختبارات سلبية للمثال المرجعي
├── tools/
│   ├── check_framework.py       # يتحقق من صحة السكلز وحدود الأحرف
│   ├── build_dist.py            # يبني نسخ كل المنصات في dist/
│   └── run_app_security_tests.py
├── .github/                     # قالب PR + خطوط CI (فحص، اختبارات، Gitleaks، Semgrep)
└── dist/                        # ⚠️ مولّد تلقائياً — لا تعدّله يدوياً
```

<div dir="rtl">

---

## 🛠️ التعديل والمساهمة

عدّل فقط في `skills/` و `policy/` و `templates/`، وبعدها شغّل:

</div>

```bash
python tools/check_framework.py          # يتحقق من صيغة السكلز والأسماء وجدول التوجيه وحدود الأحرف
python tools/build_dist.py               # يعيد بناء كل نسخ المنصات في dist/
python -m unittest discover -s tests -v  # اختبارات الصلاحيات المرجعية
```

<div dir="rtl">

الأدوات تستخدم مكتبة Python القياسية بس (Python 3.10 أو أحدث)، ما تحتاج تثبّت شي.

### إضافة سكل جديد

1. أنشئ مجلد `skills/<eng|sec>-<الموضوع>/` وفيه ملف `SKILL.md`
2. اكتب في أوله الـ frontmatter:

</div>

```yaml
---
name: eng-example-topic          # نفس اسم المجلد، أحرف إنجليزية صغيرة وشرطات، 64 حرف كحد أقصى
description: What it does and when to use it (max 1024 chars, front-load trigger words).
---
```

<div dir="rtl">

3. أضفه لجدول التوجيه في `skills/eng-core-standards/SKILL.md` (الفحص يفشل إذا نسيته)
4. شغّل الأوامر الثلاثة أعلاه، وارفع الـ PR مع `dist/` المحدّث

### الـ CI

خط [`security.yml`](.github/workflows/security.yml) يشتغل على كل PR:

| الوظيفة | وش تسوي |
|---|---|
| `framework-and-example-tests` | فحص الهيكل، بناء النسخ، الاختبارات المرجعية |
| `secret-scan` | Gitleaks على كامل تاريخ المستودع |
| `sast-semgrep` | تحليل ثابت للكود بقواعد `p/security-audit` |
| `application-security-tests` | يشتغل لما تحدد متغير `APP_SECURITY_TEST_COMMAND` لمشروعك |

> قبل الاستخدام المؤسسي، ثبّت كل `uses:` على commit SHA كامل بعد مراجعته.

---

## ⚠️ حدود لازم تعرفها

- السكلز **توجّه** سلوك الذكاء الاصطناعي، لكنها **ما تضمن** إن الكود آمن أو صحيح، وما هي شهادة امتثال. المراجعة البشرية والاختبارات الحقيقية والفاحصات هي المرجع.
- في المحادثات العادية بدون دعم سكلز، النموذج يلتزم باللي يدخل في سياقه فقط. الأفضل تستخدم Skills أو Projects أو ملفات تعليمات المشروع.
- توفّر ميزة Skills وحدود الأحرف تختلف حسب الخطة وتتغير مع الوقت، تأكد من وثائق كل منصة.
- لكل مشروع، عبّئ [`examples/ADAPTER_TEMPLATE.md`](examples/ADAPTER_TEMPLATE.md) وفعّل اختبارات أمن التطبيق وخلها إلزامية.

---

## 📖 المراجع

OWASP ASVS · OWASP Top 10 · OWASP API Security Top 10 (2023) · OWASP Top 10 for LLM Applications (2025) · NIST SP 800-63B · WCAG 2.2 · RFC 9457 · صيغة Agent Skills

## 📄 الترخيص

حدد الترخيص المناسب (مثل MIT أو Apache-2.0) وأضف ملف `LICENSE`.

</div>

---

## 🌐 English

<details>
<summary><b>Click to expand the English version</b></summary>

### Overview

A portable, stack-agnostic pack of **26 AI skills** (open `SKILL.md` / Agent Skills format) that makes any AI assistant behave like a senior software engineer **and** an application-security reviewer: it clarifies, plans, writes complete code with tests, never invents APIs/packages/test results, enforces server-side authorization and tenant isolation, keeps secrets out of code, and reports verification status honestly.

Works with **Claude, ChatGPT, Codex, Cursor, GitHub Copilot and Gemini**, in any language or framework.

### Skills

- **Core (always on):** `eng-core-standards`
- **Engineering (14):** `eng-code-quality`, `eng-architecture`, `eng-testing`, `eng-code-review`, `eng-debugging`, `eng-performance`, `eng-api-design`, `eng-database`, `eng-frontend` (WCAG 2.2, Arabic/RTL), `eng-observability`, `eng-git-workflow`, `eng-documentation`, `eng-refactoring`, `eng-devops`
- **Security (11):** `sec-authentication`, `sec-authorization`, `sec-api-security`, `sec-frontend-security`, `sec-backend-security`, `sec-data-protection`, `sec-audit-logging`, `sec-security-review`, `sec-threat-modeling`, `sec-supply-chain`, `sec-ai-llm-security`

### Install

Ready-made bundles are in [`dist/`](dist/) — see [`dist/README.md`](dist/README.md).

| Platform | Use |
|---|---|
| Claude.ai / Claude Desktop | Settings → Capabilities → Skills → upload each zip from `dist/skill-zips/` |
| ChatGPT with Skills | Skills → Create → Upload — same zips |
| Custom GPT / ChatGPT & Claude Projects / Gemini Gems | `dist/chat-projects/` (instructions ≤ 8000 chars + 4 knowledge files) |
| Any chat, no setup | Attach `dist/single-file/ALL_SKILLS.md` |
| Account-wide preferences | `dist/single-file/SHORT_INSTRUCTIONS.txt` (≤ 1500 chars) |
| Claude Code | `dist/claude-code/` → repo root |
| Codex / AGENTS.md tools | `dist/codex-agents/` → repo root |
| Cursor | `dist/cursor/` → repo root |
| GitHub Copilot | `dist/copilot/` → repo root |
| Gemini CLI | `dist/gemini-cli/` → repo root |

After copying into a repo, fill in the **Project specifics** section of the instruction file.

### Develop

```bash
python tools/check_framework.py          # validate frontmatter, names, routing, size limits
python tools/build_dist.py               # regenerate dist/
python -m unittest discover -s tests -v  # reference authorization tests
```

Edit only `skills/`, `policy/` and `templates/`; never hand-edit `dist/`. New skills must be added to the routing table in `eng-core-standards`.

### Limitations

Skills guide AI behavior; they do not guarantee secure or correct code and are not a certification. Keep human review, real tests and scanners as the source of truth. Platform features and limits change — verify against current vendor docs.

</details>
