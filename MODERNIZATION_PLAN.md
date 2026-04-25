# Personal Site Modernization Plan ("Wow Effect")

This plan is based on reviewing the current single-page implementation in `index.html`.

## 1) Vision and creative direction

### Goal
Create a premium, memorable personal brand experience that still feels fast, professional, and easy to scan for recruiters, founders, and collaborators.

### Design direction (recommended)
- **Style:** "Frosted glass + depth + subtle motion" (evolution of your current visual language).
- **Mood:** calm, confident, technical.
- **Theme system:** ship both light and dark themes with polished transitions.
- **Core promise above the fold:** "I design reliable delivery systems and ship quality at speed."

## 2) Content architecture refresh

### Keep sections but tighten messaging
- Hero: one-line value proposition + social proof strip.
- Experience: timeline with measurable outcomes (latency, reliability, cost, release cadence).
- Projects: 3 featured case-study cards (problem → solution → impact).
- Skills: grouped by domain (DevOps, QA, Backend, Platform, Leadership).
- Contact: one primary CTA and one secondary CTA.

### New sections to add
1. **"Selected Wins" mini-metrics row** (e.g., uptime, deployment frequency, incident reduction).
2. **"Case Study Spotlight" section** with expandable details.
3. **"Now" section** (what you're currently building/learning).
4. **Optional testimonial quote** from teammate/manager.

## 3) Visual and interaction upgrades

### Layout and composition
- Increase whitespace rhythm and section contrast.
- Add a diagonal/angled divider between major sections.
- Introduce sticky mini-TOC progress indicator on desktop.

### Motion strategy (tasteful)
- Scroll reveal choreography per section.
- Mouse-parallax only on hero decorative layer.
- Micro-interactions on cards/buttons (elevation + border glow).
- Respect `prefers-reduced-motion` in all animated effects.

### Typography and brand polish
- Keep `Space Grotesk` for headlines; test `Inter` or `Manrope` for body readability.
- Build a stricter typographic scale (e.g., 12/14/16/20/28/40/56).
- Define a reusable color-token system for dark/light themes.

## 4) Performance and technical quality

### Performance targets
- Lighthouse Performance >= 95 (mobile).
- LCP < 2.0s on 4G simulation.
- CLS < 0.05.

### Technical actions
- Move inline CSS/JS into versioned assets (`assets/css`, `assets/js`) for maintainability.
- Defer non-critical scripts and avoid layout thrash in animations.
- Use responsive image sizes and `loading="lazy"` for below-the-fold images.
- Add JSON-LD (`Person`) schema and stronger OpenGraph/Twitter metadata.

## 5) Accessibility and UX hardening

- Ensure color contrast AA+ for all text states.
- Improve keyboard focus visuals and skip-link behavior.
- Confirm semantic heading flow (`h1`..`h3`) and landmark usage.
- Add meaningful `aria-label` text for social/contact actions.

## 6) SEO and conversion improvements

- Rework title/description for outcome-focused search intent.
- Add canonical URL and richer social preview image.
- Add clear CTA copy: "Book a call" / "View case studies" / "Download resume".
- Add lightweight analytics event tracking for CTA clicks.

## 7) Implementation roadmap (2 weeks)

### Phase 1 — Foundation (Day 1-2)
- Information architecture + copy rewrite.
- Tokenized design system (colors, spacing, radius, shadows, motion).
- Desktop/mobile wireframes.

### Phase 2 — Core UI rebuild (Day 3-6)
- Rebuild hero, wins row, project cards, case-study spotlight.
- Add theme toggle and polished nav behavior.
- Implement responsive layout audit.

### Phase 3 — Motion + delight (Day 7-8)
- Add scroll-triggered reveals and micro-interactions.
- Add hero parallax + interactive gradient accents.
- Verify reduced-motion fallback.

### Phase 4 — Quality pass (Day 9-10)
- Accessibility audit (keyboard + screen reader basics).
- Performance optimization pass.
- SEO metadata and social card validation.

### Phase 5 — Launch and iteration (Day 11-14)
- Deploy and validate metrics.
- Collect feedback from 3-5 trusted peers.
- Ship iteration patch based on actual user behavior.

## 8) AI image generation plan (for hero/background/case cards)

Use a consistent art direction so all generated images look like one system.

### Art direction settings
- Aspect ratios: hero `16:9`, card art `4:3`, OG image `1.91:1`.
- Palette: teal/cyan/navy with soft glass highlights.
- Style keywords: "futuristic minimal", "abstract tech", "clean gradients", "depth layers".

### Prompt 1 — Hero background
"Abstract futuristic technology landscape, layered translucent glass panels, soft teal and navy gradients, subtle particle glow, high-end SaaS aesthetic, minimal, no text, cinematic lighting, ultra clean composition"

### Prompt 2 — Project card visual
"Modern DevOps workflow illustration, abstract pipelines and nodes, geometric shapes, cool blue-teal palette, depth and soft glow, minimal and professional, no logos, no text"

### Prompt 3 — OpenGraph social preview
"Premium personal brand cover image, elegant glassmorphism layers, subtle grid and gradient lighting, professional engineering identity, high contrast center focal area for overlay text"

### Prompt 4 — Contact section accent
"Friendly abstract wave forms, smooth gradients, calm tech atmosphere, clean and minimal visual, soft shadows, no text"

## 9) Acceptance checklist

- [ ] Brand feels premium and unique within first 5 seconds.
- [ ] Clear story: who you are, what you deliver, proof of impact, how to contact.
- [ ] Mobile experience equals desktop quality.
- [ ] Accessibility and performance budgets are met.
- [ ] Social share preview looks intentionally designed.

## 10) Nice-to-have stretch ideas

- Interactive "deployment pipeline" mini-animation in hero.
- Command-palette style quick navigation (`Cmd/Ctrl + K`).
- Downloadable one-page PDF resume from same design system.
- Language toggle (EN/PL) if relevant to your audience.
