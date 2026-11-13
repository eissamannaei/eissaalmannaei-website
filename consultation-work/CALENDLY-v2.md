# Calendly setup, draft 2

Changes from draft 1 after Codex review: dropped the sector question, made the form shorter, reworded the upsell question as a delivery preference, added a reschedule/no-show policy, 30-day window, recommend 45 min.

Where Claude disagrees with Codex (kept in draft 2):
- Tasks and desired outcome stay as two separate one-line questions. Merging them into one two-part prompt makes people answer only half. Both are short text, not multi-line.
- WhatsApp stays required. On the free plan Calendly cannot send automated reminders, so WhatsApp is the only reminder channel, and no-shows are the bigger risk than one extra field. The label states the benefit.

## Settings
| Setting | Draft 2 |
|---|---|
| Name | EISSA 1:1 CONSULTATION (unchanged) |
| Payment | Off (paid on Whop) |
| Duration | 45 min (owner decides 30 or 45) |
| Location | Google Meet (unchanged) |
| Availability | Friday only |
| Booking window | 30 days |
| Minimum notice | 24 hours |
| Buffer after | 15 min |
| Max meetings per day | 3 |
| Allow guests | Off |
| Booking page | Hidden from landing page; link used only as Whop checkout redirect |
| Payer check | Before each session, match invitee email to Whop Customers |

## Booking page description
حياك، تم تأكيد دفعتك. اختار الوقت اللي يناسبك يوم الجمعة، وجاوب على كم سؤال بسيط، ما ياخذ منك أكثر من دقيقتين. أراجع إجاباتك قبل الجلسة عشان ندخل مباشرة في اللي يهمك، وتطلع بخطوة واضحة تناسب شغلك.

تقدر تغيّر موعدك مرة وحدة إذا بلغتنا قبلها بـ24 ساعة. وإذا ما حضرت بدون إبلاغ، تعتبر الجلسة منتهية.

## Invitee form (after Name and Email)
1. رقم الواتساب، عشان أرسل لك تذكير ورابط الجلسة. Phone, required.
2. شو دورك الحالي؟ Radio, required: موظف / مدير فريق أو قسم / مدير إدارة / صاحب عمل / غير ذلك
3. اذكر مهمة أو مهمتين تاخذ أكثر وقتك في الشغل. One line, required.
4. شو أهم نتيجة تبي تطلع فيها من الجلسة؟ One line, required.
5. وين وصلت مع أدوات الذكاء الاصطناعي حالياً؟ Radio, required: ما بديت / أستخدم ChatGPT أحياناً / أستخدمه بشكل شبه يومي / أبني أدوات أو وكلاء
6. هل عندكم قيود على استخدام أدوات الذكاء الاصطناعي أو بيانات الشغل؟ Radio, required: لا / نعم / ما أدري
7. بعد الجلسة، أي طريق تحسّه أقرب لك؟ Radio, optional: أتعلم وأطبق بنفسي / أتعلم مع دعم ومتابعة / أفضّل أحد يبنيها معي / أبي أشوف الأنسب أول

Existing English question removed.

## Confirmation page
Calendly default (shows time, timezone, Google Meet link).
