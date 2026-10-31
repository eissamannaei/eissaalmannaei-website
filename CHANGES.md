## 2026-10-31 — Language toggle label
- Toggle now reads EN / AR in the same frame, globe icon removed.

## 2026-10-31 — Language toggle (all 12 pages)
- Toggle restyled with globe icon + accent border so it stands out; now also visible in the mobile header next to the menu button.

## 2026-10-30 — Home (en/ar): consultation funnel
- All primary CTAs -> "احجز استشارة" / "Book a consultation", opening the Typeform (mSQT5DZv) in a new tab. Removed hero "View work" button; added subline.
- "What I offer": fixed swapped descriptions on 03/04; added "Best for" + "You get" + CTA per service; 03 now an agentic system ready for production.
- New "How we work with you" (Diagnosis / Delivery / Outcome) + client-selection line.
- Agents: problem -> solution line per agent + governance line.
- New #book section (FAQ + what happens after booking) before the final CTA; floating WhatsApp button in brand blue.

## 2026-07-07 02:25 +04 — Phases B-F: repositioning, static conversion, new pages
- Converted all pages to static snapshots (pre-rendered hydrated DOM, stripped React runtime) so content is safely editable; re-added mobile menu + language toggle + contact mailto via small inline JS. Design preserved 1:1; mobile verified (no overflow).
- Home (en/ar): new hero (AI Researcher · Speaker · Agentic AI Specialist positioning + new headline/subtext); status line reframed away from training/consulting; "Expertise" -> "Focus areas"; "Consulting & training" -> "What I offer" with reframed items; removed all "coming soon"/قريباً.
- About (en/ar): new lead + 5-paragraph Story section + FAQ (4 Q&A) + FAQPage schema.
- Work (en/ar): repositioned, removed placeholders; kept real live agents.
- NEW pages: /en/speaking, /ar/speaking (7 topics) and /en/insights, /ar/insights (3 insight cards) with real content + WebPage/BreadcrumbList/Article schema.
- Nav: added Speaking + Insights to header, mobile menu, and footer on all pages; active-nav fixed on new pages.
- Contact: kept mailto form, restored submit->mailto handler (no backend per decision); social links correct.
- Cleanup: removed 62 orphaned Next RSC .txt data files and the "Add headshot" dev placeholder overlay.
- Verified: all 12 pages + llms.txt/sitemap/robots return 200; 14 JSON-LD blocks valid; no broken internal links; no placeholder/old copy; RTL correct.
- OPEN (still pending your confirm): Instagram handle kept as 'eissaalmannaei'.

## 2026-07-07 01:56 +04 — Phase A: SEO / metadata / schema / support files
- llms.txt: created at site root (AI-tool summary + key pages).
- sitemap.xml: rebuilt to 13 URLs (root + ar/en × home/about/work/speaking/insights/contact).
- robots.txt: verified (Allow: / + Sitemap) — unchanged.
- LinkedIn: fixed sitewide to https://www.linkedin.com/in/eissa-almannaei-2788bb155 (20 occurrences, visible + payload).
- Per-page <title> + meta description rewritten for all 8 pages (home/about/work/contact × en/ar); EN titles also fixed in the Flight payload so they survive hydration.
- Subpages (about/work/contact × en/ar): added canonical + og:type/site_name/url/image(+1200x630)/image:alt + twitter:image + robots index,follow; twitter:card upgraded to summary_large_image.
- JSON-LD @graph added: Person (new jobTitle[4] + knowsAbout + sameAs + email; kept award + worksFor TRENDS) + WebSite + WebPage + BreadcrumbList on home & about; WebPage + BreadcrumbList on work & contact.
- Verified via headless Chrome: titles/og/description persist after hydration on all pages; all JSON-LD valid; body intact (logo wall unaffected).
- OPEN: Instagram handle kept as current site value 'eissaalmannaei' (site + schema + llms.txt) pending confirmation vs requested 'eissamannaei'.

## 2026-07-07 01:23 +04 — P0 revisions: OG image + schema
- Created images/og-image.jpg (1200x630, site palette: accent #2d5bff on white, photo right). Served at /images/og-image.jpg (no public/ in static export). Original images/eissa.jpg untouched.
- en/ + ar/: og:image -> /images/og-image.jpg (absolute URL) + og:image:width 1200 + og:image:height 630; twitter:image -> og-image.jpg; twitter:card stays summary_large_image; og:type stays website.
- en/ + ar/: Person schema jobTitle -> [AI Researcher & Strategist, Agentic AI Systems Specialist, Institutional AI Transformation Lead]; award -> official long forms (Masdar/ADFEC; Tamkeen 5.0 FYA x ADYC; UAE Minister of AI Office).
- Note: OG image URL is absolute (best practice) rather than relative; JSON-LD Person image stays eissa.jpg (real portrait).
- 404.html / _not-found keep noindex (correct for error pages) — pending your confirmation.

# CHANGES

## 2026-07-07 01:14 +04 — P0: SEO / metadata (build-direct edits)
- index.html: removed `robots: noindex` -> `index, follow`.
- en/ + ar/: added `robots: index, follow`.
- en/ + ar/: completed Open Graph (og:type, og:site_name, og:url, og:image, og:image:alt) + twitter:image; upgraded twitter:card to summary_large_image.
- en/ + ar/: added JSON-LD Person schema (name, jobTitle, worksFor TRENDS, awards, affiliations, sameAs LinkedIn).
- en/ + ar/: added canonical links.
- Note: OG image path is /images/eissa.jpg (no public/ in a static export).
- robots.txt already present with `Allow: /` + Sitemap (no change needed).
