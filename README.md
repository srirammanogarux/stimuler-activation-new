# Stimuler · India Onboarding

Interactive prototype of the revamped chat onboarding for **Stimuler** (India), rebuilt from Figma and iterated on section by section.

**Live:** https://india-onboarding.vercel.app

No build step, no dependencies — open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
```

## What it is

A single-page vanilla JS state machine that plays the whole onboarding inside a phone mockup: Sarah types in with realistic voice pacing, you tap real options and inputs, record a mocked speaking test, get scored, drill your pronunciation, and land on the paywall.

## The flow

| # | Section | Notes |
|---|---------|-------|
| 1 | Intro | Sarah's greeting + animated bitmoji with twinkling stars |
| 2 | Native language | Indian languages, Hindi first |
| 3 | App language | Switches the whole flow to romanized copy |
| 4–5 | Name · Phone | Real typed input, country code follows the language |
| 6–7 | Attribution · Goal | Goal drives the paywall headline |
| 8 | Testimonials | **A/B:** text carousel vs. video carousel + story player |
| 9 | Level | Drives the speech meter target |
| 10 | Reading test | Conversation mic: orb → waveform pill → tick, then a success toast |
| 11 | Award | Google Play "Best AI App" |
| 12 | Speech meter | Animated CEFR ladder, then the gold target beat |
| 13–14 | Fix pronunciation · Practice | Two words, score climbs 52→80% |
| 15 | Graph → Paywall | Gold curve animates, then gels into the full paywall |
| 16–17 | Gift · Offer paywall | Tap the box → 50% coupon → discounted paywall + plans sheet |

## Review panel

On desktop a side panel deep-links into any point of the flow. All state is in the URL:

```
?step=practice&lang=ta&lvl=advanced&variant=b
```

- `step` — jump straight to any section (everything before it fast-forwards)
- `lang` — `en · hi · mr · ta · te · kn · ml`
- `lvl` — `beginner · intermediate · advanced` (speech meter)
- `variant` — `a` (text testimonials) · `b` (video testimonials)

## Design system

`tokens.css` is the single source of truth; `styles.css` holds layout and component anatomy only.

- **Interactive** — one colour, periwinkle `#6C63FF`. Every tappable fill uses it.
- **Progress & reward** — gold `#D9A24A`. Never used for a "tap me" affordance.
- **Feedback** — green for success, amber for "needs work".

Two live specs:

- `styleguide.html` — the full component inventory (bubbles, chips, options, inputs, mic, cards, practice states) rendered from the tokens
- `graph-gift-colors.html` — the gold ramp and every part of the graph, gift and paywall, with literal hex for Figma

## Localization

Six Indian languages plus English. Localized copy is **romanized** — Latin script, the way people actually type on WhatsApp ("Aapka naam kya hai?", not Devanagari).

**CTAs are never localized.** Buttons, links and control labels stay English in every language; only Sarah's conversation, headings and descriptions translate.

## Files

```
index.html              flow markup (all screens)
app.js                  chat engine + flow script + takeover sequences
i18n.js                 copy for 7 languages
tokens.css              every colour decision
styles.css              layout + component anatomy
styleguide.html         component spec
graph-gift-colors.html  colour spec for Figma
assets/                 art, flags, icons, paywall + gift art
assets/videos/          testimonial footage
```

## Notes

- All voice, mic and scoring behaviour is mocked; the mic never records.
- Testimonial personas and quotes are placeholders for design review, not real endorsements.
- Prices are illustrative.
