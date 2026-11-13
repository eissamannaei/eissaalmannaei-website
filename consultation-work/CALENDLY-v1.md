# Calendly setup, draft 1

## Context
- Funnel: Instagram (bio / DM keyword / stories) > landing page > Whop checkout (paid, 150 USD, one-time) > Whop "Checkout redirect" > this Calendly event > 1:1 diagnostic consultation on Google Meet > upsell (group hybrid program, or done-for-you build 5,000 USD+).
- Audience: Gulf (mostly UAE) employees, department managers and business owners who want to be "Number 1 at AI" in their job or company. Arabic-speaking, mobile, Gulf dialect.
- Owner: Eissa Almannaei, Emirati AI trainer/researcher. Calendly is on the free plan (shows "Upgrade plan").

## Current state of the event (observed)
- Name: EISSA 1:1 CONSULTATION, slug /eissa-1-1-consultation, One-on-One, violet.
- Duration 30 min, Google Meet.
- Availability: Friday and Sunday (weekly hours 16:00-21:00 on at least one of them). Booking window 60 days, min notice 4 hours.
- Description: empty.
- Limits and buffers: none set.
- Invitee form: name, email; guests allowed; 1 optional multi-line question "Please share anything that will help prepare for our meeting."
- Payment: 170 USD collected through PayPal.
- Notifications: calendar invitations only.
- Confirmation page: default Calendly confirmation page.

## Owner decisions already made
- Keep the existing event and its name.
- Remove Calendly payment (payment happens on Whop).
- Availability: Friday only.

## Proposed changes

### Settings
| Setting | Proposed |
|---|---|
| Payment | Off |
| Description | Short Arabic text (below) |
| Availability | Friday only (turn Sunday off) |
| Duration | Keep 30 min, or 45 min (owner decision) |
| Minimum notice | 24 hours (time to read answers) |
| Buffer | 15 min after |
| Meeting limit | Max 3 per day |
| Allow guests | Off (it is a 1:1 diagnostic) |
| Booking page | Hidden/secret, only reachable via Whop redirect |
| Booking link visibility | Do not share publicly; verify payer email in Whop before each session |
| Reminders | Email reminder 24h and 1h before (if available on free plan) |

### Description (Arabic, shown on the booking page)
شكرا على حجزك. اختار الموعد اللي يناسبك يوم الجمعة، وجاوب على أسئلة قصيرة عن شغلك (أقل من دقيقتين). أقرأ إجاباتك قبل الجلسة عشان ندخل مباشرة في التشخيص.

### Invitee questions (Arabic, in this order)
1. رقم الواتساب (Phone, required) - for reminders and follow-up.
2. شو دورك الحالي؟ (Radio, required): موظف / مدير قسم / مدير إدارة / صاحب عمل / غير ذلك
3. في أي قطاع تشتغل؟ (Radio, required): حكومي / شبه حكومي / خاص / غير ذلك
4. شو أكثر 3 مهام تاخذ من وقتك كل أسبوع؟ (Multiple lines, required)
5. لو نجحت الجلسة، شو تبي يكون تغيّر في شغلك بعد 3 شهور؟ (Multiple lines, required)
6. شو علاقتك الحالية بأدوات الذكاء الاصطناعي؟ (Radio, required): ما بديت / أستخدم ChatGPT أحياناً / أستخدمه يومياً / أبني أدوات أو وكلاء
7. هل في قيود في جهتك على استخدام أدوات الذكاء الاصطناعي أو البيانات؟ (Radio, required): لا / فيه قيود / ما أدري
8. لو لقينا الحل المناسب، تفضّل تتعلم وتبنيه بنفسك، ولا نبنيه معك؟ (Radio, optional): أتعلم وأبني بنفسي / نبنيه مع بعض / ما قررت
- Remove the existing generic English question.

### Confirmation page
Keep Calendly confirmation page (free plan may not allow redirect).
