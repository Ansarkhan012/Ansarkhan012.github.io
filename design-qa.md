# Ansar Games website — design QA, 17 November 2026

final result: passed

## Visual target aur evidence

- Selected visual truth: option 2, `C:/Users/ansar/.codex/generated_images/01a1e356-5221-7f52-948b-d80fea98eecc/exec-dbd4b650-8293-473e-bf65-4416206e4b80.png`.
- Source image: 1024 × 1536 pixels; unframed desktop concept.
- Implementation: `D:/word_jars/website-design/2026-11-17/desktop-final.png`, 1008 × 1762 pixels, full-page browser capture.
- CSS viewport 1024 × 1536; device pixel ratio approximately 1. Browser capture excludes its scrollbar. Source ko comparison mein 1008 × 1512 par proportional resize kiya; implementation ko stretch nahi kiya.
- State: homepage, top, English, studio light palette, no hover. Full-view combined evidence: `comparison-final.jpg`; focused header/hero combined evidence: `comparison-hero-final.jpg`, isi evidence directory mein.
- Mobile visual evidence: `mobile-final.png`, browser viewport 390 × 844. Source ne mobile mock nahi diya; mobile behavior desktop direction ka responsive adaptation hai.
- Game-page visual checks: `word-jars-mobile.jpg`, `block-bloom-mobile.png`.

## Comparison history

1. Pehle comparison (`comparison-v1.jpg`) mein [P2] studio wordmark aur game headings chhoti theen; headline ka scale aur position target se door tha. Brand size, headline size/weight/tracking, game heading sizes aur hero position adjust ki.
2. Pehle mobile capture (`mobile-v1.png`) mein [P2] descriptions artwork ke paas narrow column mein reh rahi theen. Mobile grid mein description aur detail link ko full width di. Revised evidence `mobile-final.png` mein text khula aur readable hai.
3. Final full-view aur focused combined comparisons khol kar typography, section order, colour balance, artwork, buttons aur text inspect kiya. Koi actionable P0/P1/P2 mismatch baqi nahi mila.

## Required fidelity surfaces

- **Fonts / typography:** locally hosted variable Outfit use hua. Weight, headline hierarchy, two-line desktop headline, game titles aur compact navigation target direction ko follow karte hain. Mock ka exact font identify nahi tha; Outfit intentional closest practical match hai. Narrow layouts mein title aur body wrap inspect kiye.
- **Spacing / layout:** desktop two-column hero, navy featured Zen Sort band, two upcoming cards aur logo-led studio section rakhe. Phone par artwork stack aur card body full width hoti hai. Footer target se lamba hai kyunke teen real policies ko direct access dena zaroori hai.
- **Colours / tokens:** warm ivory `#fffaf2`, navy `#0b1d3b`, orange `#ff4b16`, yellow `#ffd325`. Studio palette intentional light hai; game pages apne existing light/dark themes rakhte hain. Focus outline maujood hai.
- **Images / quality:** hero aur AG mark built-in ImageGen se target reference ke saath generate hue. Original game icons source files se reuse hue; hero WebP aur transparent logo WebP optimized hain. Custom SVG/CSS drawings se logo ya hero replace nahi kiya. Arrow Bootstrap Icons ka licensed source asset hai. Small game cards mein authentic app-icon backgrounds rakhna intentional hai.
- **Copy / content:** hero copy, games, availability aur studio statement target follow karte hain. Homepage descriptions short rakhi hain; numerical marketing claims copy nahi kiye. Zen Sort ka real store URL hai. Block Bloom / Word Jars coming soon hain. Ratings, downloads ya awards invent nahi kiye. Policy body text comparison teenon files mein unchanged pass hua.

## Functional verification

- Homepage browser checks: 320, 390, 620, 768, 1024, 1440 CSS pixels. Koi horizontal page overflow ya broken image nahi mila. Evidence `responsive-home.json`.
- Teen game pages aur teen policy pages: har ek 320 aur 768 pixels par browser-rendered check. Koi page-level horizontal overflow ya missing image nahi mili. Evidence `page-checks.json`. Policy tables aur screenshot shelf apne container mein scroll karte hain.
- Homepage puzzle CTA, Zen Sort detail journey, game-to-policy navigation, home return, Block Bloom detail link, Studio, Support aur Privacy anchors exercise kiye.
- Mail support ka `mailto:` destination aur teen direct policy destinations inspect kiye; email send nahi ki.
- Browser error/warning log check mein koi entry nahi mili.
- Static HTML check: 7 pages, 147 local asset/link/fragment references, zero missing destinations. Evidence `static-checks.json`.
- Teen privacy policies ke normalized body text original repository se match hue.
- Developer logo export: 512 × 512 RGBA PNG; 1024 PNG aur transparent master bhi available.

## WHAT / WHY / HOW / HOW VERIFIED

**WHAT:** homepage, studio branding, responsive cards, favicon, shared game/policy header logo aur export pack.

**WHY:** purane narrow desktop cards aur generic studio identity ko selected visual direction ke mutabiq behtar banana.

**HOW:** existing static HTML/CSS architecture mein `studio.css` aur optimized assets add kiye. App pages ka existing content/art direction aur privacy texts preserve kiye. Koi runtime framework, analytics ya third-party font request add nahi ki.

**HOW VERIFIED:** combined visual comparisons, rendered responsive checks, navigation checks, browser logs, local reference validation aur original-policy text comparison.

## Follow-up polish aur limits

- [P3] Mock ke edge doodles aur miniature Google Play triangle repeat nahi kiye; actual store CTA text aur URL clear hain. Yeh use ko block nahi karta.
- [P3] Exact mock font aur hand-rendered artwork texture pixel-identical nahi hain; approved composition aur identity follow hoti hai.
- Physical phone, Safari, Firefox, assistive technology aur actual Play Console upload test nahi kiya. Yeh browser viewport checks real-device validation nahi hain.
- GitHub Pages deployment is redesign verification ka hissa nahi tha. Local reviewed files aur running preview deliver kiye ja rahe hain.

## Implementation checklist

- [x] Selected direction implemented.
- [x] Hero/logo production assets placed.
- [x] Mobile card reading-width issue fixed.
- [x] Local routes and policy text checked.
- [x] Full-view and focused design comparison completed.
- [x] Logo exports prepared; upload still user/account action hai.
