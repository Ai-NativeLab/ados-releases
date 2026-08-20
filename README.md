# ados-releases

إصدارات جاهزة للتثبيت (`.whl`) من أدوات `Agentic Delivery OS` — لا كود مصدري هنا.

المصدر الحقيقي: [`Agentic_Delivery_OS`](https://github.com/Ai-NativeLab) (المستودع الأساسي).
هذا المستودع للتوزيع فقط، عبر [Releases](../../releases).

## الحزم المتاحة

| الحزمة | لمن | الأوامر |
|---|---|---|
| `ados-exec` | فرق التنفيذ — تشغّل `epic-runner`/`ticket-executor`/`ticket-reviewer` على مستودعها فقط | `validate` · `readiness` · `sync` |

## التثبيت

```bash
pip install https://github.com/Ai-NativeLab/ados-releases/releases/download/<tag>/<الملف>.whl
```

استبدل `<tag>` برقم الإصدار من صفحة [Releases](../../releases)، و`<الملف>` باسم ملف `.whl` المرفق به.

## الترقية

نفس الأمر بعد تحديث الرابط لإصدار أحدث، أو:

```bash
pip install --upgrade https://github.com/Ai-NativeLab/ados-releases/releases/download/<tag-جديد>/<الملف>.whl
```
