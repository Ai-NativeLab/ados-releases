# ados-releases

إصدارات جاهزة للتثبيت (`.whl`) من أدوات `Agentic Delivery OS` — لا كود مصدري هنا.

المصدر الحقيقي: مستودع `Agentic_Delivery_OS` الأساسي. هذا المستودع للتوزيع فقط، عبر
[Releases](../../releases). **مستودع عام** — لا كود حسّاس هنا (طبقة الإدارة مُستبعدة
تمامًا من كل حزمة هنا بتصميمها)، فلا حاجة لتوكن عند التثبيت.

## الحزم المتاحة

| الحزمة | لمن | الأوامر |
|---|---|---|
| `ados-exec` | فرق التنفيذ — تشغّل `epic-runner`/`ticket-executor`/`ticket-reviewer` على مستودعها فقط | `validate` · `readiness` · `sync` |

## التثبيت

```bash
pip install https://github.com/Ai-NativeLab/ados-releases/releases/download/ados-exec-v0.1.0/ados_exec-0.1.0-py3-none-any.whl
```

تحقّقتُ من هذا الأمر فعليًا في بيئة نظيفة معزولة قبل نشره هنا.

## الترقية

نفس الأمر بعد تحديث رقم الإصدار في الرابط لأحدث نسخة على [صفحة Releases](../../releases)، أو:

```bash
pip install --upgrade <رابط الإصدار الأحدث>
```
