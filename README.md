# ados-releases

إصدارات جاهزة للتثبيت (`.whl`) من أدوات `Agentic Delivery OS` — لا كود مصدري هنا.

المصدر الحقيقي: مستودع `Agentic_Delivery_OS` الأساسي. هذا المستودع للتوزيع فقط، عبر
[Releases](../../releases).

## الحزم المتاحة

| الحزمة | لمن | الأوامر |
|---|---|---|
| `ados-exec` | فرق التنفيذ — تشغّل `epic-runner`/`ticket-executor`/`ticket-reviewer` على مستودعها فقط | `validate` · `readiness` · `sync` |

## التثبيت

**المستودع خاص** — رابط `.../releases/download/...` العادي بلا توكن يفشل بـ 404. اختر
إحدى الطريقتين:

**١) عبر توكن GitHub (سطر أوامر — تحقّق فعليًا، يعمل):**

```bash
curl -sL -H "Authorization: Bearer $GITHUB_TOKEN" -H "Accept: application/octet-stream"   "https://api.github.com/repos/Ai-NativeLab/ados-releases/releases/assets/522880097"   -o ados_exec-0.1.0-py3-none-any.whl
pip install ados_exec-0.1.0-py3-none-any.whl
```

**مهمّ:** اسم الملف الناتج عن `-o` يجب أن يطابق اسم ملف الـ wheel الأصلي بالضبط
(`ados_exec-0.1.0-py3-none-any.whl`) — pip يرفض أي اسم آخر بخطأ
`Invalid wheel filename`، حتى لو كان المحتوى صحيحًا.

رابط الـ API أعلاه (`api.github.com/.../releases/assets/<id>`) هو الصحيح مع curl —
لا رابط `github.com/.../releases/download/...` العادي، فذاك يحتاج جلسة متصفح لا توكنًا
في الترويسة. رقم `<id>` يظهر في تفاصيل كل إصدار على [صفحة Releases](../../releases)
(أو عبر `GET /repos/Ai-NativeLab/ados-releases/releases`).

**٢) تنزيل يدوي من المتصفح** (أي عضو في المؤسسة مسجَّل دخوله يرى الملف تلقائيًا):
افتح صفحة [الإصدار](../../releases)، نزّل ملف `.whl`، ثم:

```bash
pip install ./ados_exec-0.1.0-py3-none-any.whl
```

## الترقية

كرّر خطوة التثبيت بعد تحديث رقم الإصدار/رقم الـ asset لأحدث نسخة على صفحة Releases.
