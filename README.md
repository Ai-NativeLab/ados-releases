# ados-releases

إصدارات جاهزة للتثبيت (`.whl`) من أدوات `Agentic Delivery OS` — لا كود مصدري هنا.

المصدر الحقيقي: مستودع `Agentic_Delivery_OS` الأساسي. هذا المستودع للتوزيع فقط، عبر
[Releases](../../releases).

## الحزم المتاحة

| الحزمة | لمن | الأوامر |
|---|---|---|
| `ados-exec` | فرق التنفيذ — تشغّل `epic-runner`/`ticket-executor`/`ticket-reviewer` على مستودعها فقط | `validate` · `readiness` · `sync` |

## التثبيت

**المستودع خاص** — تنزيل ملف `.whl` مباشرة بلا توكن (`pip install <رابط>`) لن يعمل (404).
اختر إحدى الطريقتين:

**١) عبر توكن GitHub (سطر أوامر، قابل للنسخ في سكربت تركيب):**

```bash
curl -sL -H "Authorization: Bearer $GITHUB_TOKEN" -H "Accept: application/octet-stream"   "<رابط asset من صفحة الإصدار — انسخه من Releases>" -o ados_exec.whl
pip install ados_exec.whl
```

رابط الـ asset الصحيح للاستخدام مع curl هو رابط الـ API (`api.github.com/repos/.../releases/assets/<id>`)
لا رابط `github.com/.../releases/download/...` العادي — الأخير يحتاج جلسة متصفح لا توكنًا في الترويسة.

**٢) تنزيل يدوي من المتصفح** (أي عضو في المؤسسة مسجَّل دخوله يرى الملف تلقائيًا):
افتح صفحة [الإصدار](../../releases)، نزّل ملف `.whl`، ثم:

```bash
pip install ./ados_exec-٠.١.٠-py3-none-any.whl
```

## الترقية

كرّر خطوة التثبيت بعد تحديث رقم الإصدار/رابط الـ asset لأحدث نسخة على صفحة Releases.
