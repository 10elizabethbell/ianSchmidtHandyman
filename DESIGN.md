---
name: Ian Schmidt
description: One-man yard work, hauling, handyman and holiday lights in Toms River, NJ. Leaves now, lights next.
colors:
  pine: "#183a2c"
  night: "#132d23"
  deep: "#10261d"
  kraft: "#e6d2aa"
  bark: "#2b1d12"
  bark-2: "#5b4330"
  cream: "#f6ecd8"
  sage: "#c3d5c1"
  rust: "#b8441e"
  rust-hi: "#9e3615"
  amber: "#e3922c"
  gold: "#f2bf45"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.7rem, 12.4vw, 6rem)"
    fontWeight: 900
    lineHeight: 0.92
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2rem, 8.4vw, 3.4rem)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.34rem"
    fontWeight: 800
    lineHeight: 1.2
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.34rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "0.06em"
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.06rem"
    fontWeight: 400
    lineHeight: 1.55
rounded:
  pill: "999px"
  circle: "50%"
  field: "12px"
  panel: "16px"
  focus: "6px"
spacing:
  gutter: "16px"
  max: "1180px"
  sec: "64px"
  sec-wide: "104px"
  button-gap: "12px"
  chip-gap: "10px"
components:
  button-fill:
    backgroundColor: "{colors.rust}"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "56px"
  button-fill-hover:
    backgroundColor: "{colors.rust-hi}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.cream}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "56px"
  button-line-on-kraft:
    backgroundColor: "transparent"
    textColor: "{colors.bark}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "56px"
  service-row:
    textColor: "{colors.bark}"
    typography: "{typography.title}"
    height: "60px"
    padding: "8px 0"
  service-row-arrow:
    textColor: "{colors.bark}"
    rounded: "{rounded.circle}"
    size: "40px"
  service-row-arrow-hover:
    backgroundColor: "{colors.rust}"
    textColor: "#ffffff"
  chip:
    backgroundColor: "rgba(246,236,216,.05)"
    textColor: "{colors.cream}"
    rounded: "{rounded.pill}"
    padding: "0 16px"
    height: "46px"
  chip-checked:
    backgroundColor: "{colors.cream}"
    textColor: "{colors.pine}"
  input:
    backgroundColor: "rgba(246,236,216,.07)"
    textColor: "{colors.cream}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "52px"
  step-number:
    backgroundColor: "{colors.pine}"
    textColor: "{colors.gold}"
    rounded: "{rounded.circle}"
    size: "48px"
  header:
    backgroundColor: "{colors.pine}"
    textColor: "{colors.cream}"
    height: "64px"
  footer:
    backgroundColor: "{colors.deep}"
    textColor: "{colors.sage}"
---

# Design System: Ian Schmidt

## Overview

**Creative North Star: "The Job Itself"**

This is a one-man yard business, and the site shows the work instead of describing it. On the first screen you get a pine-green dusk over a mown lawn buried in maple, oak and elm leaves, and you rake them clear with a finger or the mouse. Further down, C9 bulbs hang on a shingled roofline at night and swing when you pass over them or tap. Between these two scenes, the sections you read sit on leaf-bag kraft paper. The palette comes from the yard: pine and night greens, rust, amber and gold leaves, kraft, bark brown, cream.

Type does the heavy lifting. Headings are huge, uppercase and weight 900, set in the system stack, with tight tracking. There are three interaction shapes: round pill buttons, arrow-circle service rows and circular step numbers. There are no cards, no stock photos, no tool icons and no service-card grid. The page is phone-first and dense with intent, built around one action: text Ian.

**Key Characteristics:**
- Two canvas scenes carry the identity: the leaf lawn (hero, plus a smaller strip at the foot of the estimate section) and holiday lights on a roofline.
- Dark-green sections (pine, night, deep) alternate with kraft reading sections.
- Heavy uppercase system type. No webfonts.
- Round geometry everywhere you touch: pills, circles, 12px fields.
- Flat surfaces. Depth comes only from the canvases and one soft button shadow.
- First-person owner voice, and only Ian's own facts.

## Colors

The palette is the yard at dusk: deep evergreen grounds, warm kraft paper, and fallen-leaf warmth used as accents.

### Primary
- **Leaf Rust** (rust): the action color. It fills every primary pill button, the hover/active fill of the service-row arrow circle, and the caret on kraft. White text on rust passes AA.
- **Pressed Rust** (rust-hi): hover state of the filled button only.

### Secondary
- **Bulb Gold** (gold): the light accent on dark grounds. Used for the second line of the hero headline ("handled."), the phone icon in the header, step numbers, every gold focus/hover outline on dark sections, and the input caret.
- **Maple Amber** (amber): text selection highlight. Its wider role is inside the leaf canvas palette.

### Neutral
- **Pine** (pine): header, hero top, estimate section, step-number discs. Also the theme-color.
- **Night Pine** (night): the holiday-lights section ground.
- **Deep Pine** (deep): footer and the html background behind overscroll.
- **Leaf-Bag Kraft** (kraft): body background and the reading sections (services, me, photos).
- **Bark** (bark): body text on kraft, outlined buttons on kraft, arrow circle default.
- **Worn Bark** (bark-2): service group labels and step descriptions on kraft.
- **Cream** (cream): text on dark grounds, outlined button stroke on dark, checked chip fill.
- **Sage** (sage): secondary text on dark grounds (header tagline, lights and estimate intros, notes, footer).

Translucent derivatives are written inline as rgba of their parent: bark at .14/.18/.35 for kraft hairlines and the arrow ring; cream at .05/.07/.4/.7 for chip and field fills, their strokes, and the outlined-button stroke on dark.

### Canvas palettes (in-script, not CSS tokens)
- **Leaves**: eight gradient pairs (dark, light): `#9b2d16/#cc4c22`, `#c2541e/#e8852d`, `#d6871f/#f1b03a`, `#dea52a/#f4cd5e`, `#7c4320/#a7652e`, `#b03a1c/#df6e2b`, `#8d5823/#c08a3b`, `#a8441c/#d9732e`. Leaf backs mix toward `#ead8ab`. Veins and stems mix toward bark.
- **Lawn**: base gradient `#5a8a4c` > `#3e6e39` > `#2a552b`, with blade strokes in five rgba greens. Far-edge grass fringe in `#5f9150`, `#4a7d42`, `#78a85e`. The CSS fallback behind the canvas is `#4f7f46` > `#3a6a37` > `#2e5a2e`.
- **Mulch bed** (hero only): fill `#43281a`, chips in `#6e4329`, `#2f1a0e`, `#85573a`, `#4f2f1c`, `#9a6a45`.
- **C9 bulbs**: `#ff4a36` red, `#3ddc6a` green, `#ffb02e` yellow, `#4f8dff` blue, `#ff7a1f` orange, `#fff0c2` warm white. Each bulb has a `#fffbe8` hot core, an additive radial glow, and a `#1f3a2b` socket.
- **Roofline**: shingles `#3a3833`, `#33312c`, `#2c2a26`, `#403d37`. Fascia gradient `#ece6d6` > `#d3cbb8` > `#8f8a7c`. Wire `#2d4a37`, clips `#d9d3c4`.

### Named Rules
**The Rust Means Text Rule.** Rust fills mean "this opens a text to Ian". Spend it on the primary pill buttons and the arrow-circle hover, nowhere else.

**The Gold On Dark Rule.** Gold is the focus and highlight color on pine and night grounds. On kraft, focus switches to rust (outlined buttons, arrow rings), because gold disappears on kraft.

**The Ground Alternation Rule.** Sections alternate between dark greens and kraft: pine header and hero, kraft services, night lights, kraft me and photos, pine estimate, deep footer. A new section takes whichever ground continues the alternation.

## Typography

**Display Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** the same stack

**Character:** This is a deliberate house choice. PRODUCT.md fixes a system font stack because visitors arrive in Facebook's in-app browser on phones. Personality comes from weight (900), uppercase and tight tracking, not from the face.

### Hierarchy
- **Display** (900, clamp(2.7rem, 12.4vw, 6rem), 0.92, -0.035em, uppercase): hero h1 only. Its second line is a block span in gold. From 900px it grows to clamp(4.5rem, 8.6vw, 7.5rem).
- **Headline** (900, clamp(2rem, 8.4vw, 3.4rem), 1, -0.02em, uppercase, balanced wrap): every section h2.
- **Title** (800, 1.34rem): service row labels. Step titles are 900, 1.06rem, uppercase. Wordmark is 900, 1.06rem, uppercase, +0.01em.
- **Lead** (400, 1.34rem, max 34-42ch): the paragraph right under each h2. Sage on dark, bark on kraft.
- **Body** (400, 17px, 1.55): the base. The hero promise is clamp(1.05rem, 4.6vw, 1.25rem) at 1.45, max 34ch.
- **Label** (900, 0.95rem, +0.06em, uppercase): service group h3 in bark-2 with a 2px bark hairline below. Form legends and labels are 800, 1.06rem, sentence case.
- **Small** (0.82rem): the header subtitle and the list group labels only. Form notes, errors, the canvas hint and the copy-fallback line use the 17px body size.
- Buttons: 800, 1.06rem, line height 1.1. The phone number uses tabular numerals.

### Named Rules
**The Weight Not Face Rule.** Hierarchy comes from 900 uppercase against 400 sentence-case body. Never add a webfont or a second family.

**The Uppercase Is For Headings Rule.** Uppercase belongs to h1-h3, step titles, the wordmark and the footer name. Body copy, buttons, labels and chips stay in sentence case.

## Layout

- **Phone-first.** Base styles target about 360px. One column. The gutter is 16px (`--gut`), centered inside a 1180px max (`--max`).
- **Breakpoints:** 374px max-width (smaller phone number and logo), 560px (button pairs go inline, the header tagline goes onto one line, the lights string goes from 2 swags to 3), 900px (sections grow from 64px to 104px padding, service groups go 2-up with a 56px gap, steps go 3-up, the hero grows), 1024px (the estimate splits into intro plus form, 1fr / 1.15fr, 72px gap). Canvases switch phone/desktop tunables at 700px canvas width.
- **Hero:** fills the viewport below the header, `calc(100svh - 64px)`, capped at 860px from 900px. Copy sits on top, and the lawn canvas takes the remaining flex space (230-440px tall, at least 300px on desktop).
- **Rhythm:** sections pad 64px / 104px. h2 to lead is 16-18px. Lead to buttons is 26px. Button stacks use a 12px grid gap. Chips have a 10px gap. Form fields have a 22px gap.
- **Line length:** reading copy is capped at 34-42ch.

## Elevation & Depth

Surfaces are flat. There are no cards and no layered panels. Depth lives in the canvases: perspective-scaled leaves with ground shadows, additive bulb glow, and the shadow band under the roof gutter. CSS shadow is limited to two values.

### Shadow Vocabulary
- **Button lift** (`box-shadow: 0 8px 18px -10px rgba(8,20,14,.55)`): the filled rust button only.
- **Hint legibility** (`text-shadow: 0 1px 3px rgba(16,38,29,.9), 0 0 10px rgba(16,38,29,.6)`): the "Drag to rake" hint over the lawn. It is there for legibility, not decoration.

`--shadow` is declared on :root but no rule uses it.

### Named Rules
**The Canvas Holds The Depth Rule.** Don't add shadows to UI chrome. If something needs to read as dimensional, it belongs to a scene.

## Shapes

Everything you touch is round. Buttons and chips are full pills (999px). Arrow rings and step numbers are perfect circles (50%). Text fields are 12px. The sent-message panel is 16px. Focus rings on text links get 6px corners. Section edges are straight. On kraft, list structure comes from hairlines: 1px between service rows and 2px under group labels. The leaf mark (a maple silhouette SVG) is the only logo.

## Components

### Buttons
Confident, thumb-sized pills.
- **Shape:** full pill (999px), at least 56px tall, 24px side padding, icon and label with a .55em gap, 2px border.
- **Filled:** rust with white text and the button-lift shadow. Hover turns it rust-hi. Active scales to .98. Every filled button starts a text, so it carries the speech-bubble icon.
- **Outlined:** transparent with cream text and a cream stroke at .7 on dark grounds. On hover the stroke goes full cream over a .08 cream wash. On kraft (`.on-kraft`) it becomes bark text with a bark stroke and a .06 bark hover wash.
- **Focus:** 3px gold outline, offset 3px. On kraft the outline is rust.
- **Pairs:** stacked full-width on phones, inline (auto auto, left-aligned) from 560px. The form submit is full-width. When it is the submit or the copy button, hover also adds a gold 2px outline.

### Service rows (signature list)
Each row is a link that opens a text with a service-specific prefill.
- 60px minimum height, 8px vertical padding, 800 / 1.34rem label, 1px bark hairline at .14 between rows.
- The trailing 40px arrow circle has a 2px bark ring at .35.
- **The Only The Arrow Moves Rule.** On hover, focus and active, the row itself does not change. No background, no underline, no shadow, no outline. Only the arrow circle fills rust with a white arrow. On focus-visible the arrow also gets a 3px rust ring.

### Chips
Multi-select checkboxes in the estimate form.
- **Style:** pill, 46px tall, 16px padding, 1.5px cream stroke at .4 over a .05 cream wash, weight 700.
- **Checked:** solid cream with pine text and a 16px check icon.
- **Hover / focus:** a 2px gold outline, offset 2px. Checking is the only fill change.

### Inputs / Fields
- **Style:** cream text, .07 cream wash, 1.5px cream stroke at .4, 12px radius, 14px 16px padding, 52px minimum height. The textarea starts at 104px and resizes vertically. Placeholder is sage at .8. The caret is gold.
- **Hover / focus:** 2px gold outline, offset 2px. The fill does not change.
- **Error:** an inline sentence below the field (`#ffcf9a`, 700, 1.06rem), written in Ian's voice, plus `aria-invalid`. Focus moves to the first missing field.

### Numbered steps
Three steps from text to done. Each has a 48px pine disc with a gold 900 numeral (CSS counter), an uppercase 900 title, and a bark-2 one-liner. They stack on phones and go 3-up from 900px.

### Navigation
- **Header:** pine bar, 64px. Wordmark (leaf mark, uppercase name, sage tagline) on the left. The phone number is on the right: a tel link with a gold phone icon, weight 800, underline on hover, 44px tap target. There are no nav links.
- **Footer:** deep ground, cream uppercase name, sage service line. Contact links are the phone and Facebook, cream 700, 44px targets, underline on hover, gold focus ring.

### Leaf lawn (signature canvas)
- Hero (`sky:34`, mulch bed, gusts, hint) and the strip at the foot of the estimate section (`sky:30`, no mulch, gusts, `scale:.55`).
- **Rake:** the mouse rakes on hover. Touch rakes while the finger is down (`touch-action:none` on the hero). Fast strokes flip leaves into the air.
- **Idle:** after `IDLE_AFTER` (4s) without touch, wind gusts sweep across every 2.4-4.8s.
- Tunables live at the top of the leaves IIFE: `DENSITY`, `MAX_LEAVES`, `LEAF_PX`, `RAKE_R`, `GROUND_FRICTION`, `GUST_EVERY`, `IDLE_AFTER`, `MULCH`. Change behavior there, not in the physics.
- Three leaf shapes (maple 50%, oak 30%, elm 20%) are pre-rendered to 64px sprites with front and back faces. The lawn texture is baked once per size.
- The hint ("Drag to rake the leaves", or "Sweep the mouse across..." on fine pointers) fades out on first touch.

### Holiday lights (signature canvas)
- A night-green band (176px, 200px from 900px) with a shingled roof edge, fascia and clips at the top. A swagged wire hangs 2-4 swags depending on width. C9 bulbs repeat the six colors in order.
- **Swing:** a passing pointer pushes bulbs by its horizontal velocity. A tap swings and brightens the bulbs within 80px. Bulbs drift a little in the wind.
- Tunables live at the top of its IIFE: `SPACING`, `SAG`, `SPRING`, `DAMP`, `PUSH`, `TAP_R`, `COLORS`.
- `touch-action:pan-y`, so the page still scrolls through it. It is decorative (`aria-hidden`).

### Motion rules
**The One Loop Rule.** Every animated scene registers with the shared `Loop` (one requestAnimationFrame, dt clamped to 33ms). Never start a second rAF.

**The Off-Screen Sleep Rule.** An IntersectionObserver (80px margin) marks scenes visible. The loop stops when none are visible and wakes on input.

**The Still Frame Rule.** Under `prefers-reduced-motion`, each canvas draws one static frame and redraws only on resize. Smooth scroll is off too. Device pixel ratio is capped at 1.5.

UI transitions stay short: .2s on colors, .15s on chips, .12s on press scale, .6s on the hint fade.

## Do's and Don'ts

### Do:
- **Do** route every call to action through `data-sms` with one number (+17323004510) and a job-specific prefilled body. Every filled button carries the speech-bubble icon.
- **Do** keep 44px minimum tap targets, and 56px for buttons.
- **Do** write in Ian's first-person voice ("I", "me", "Text me"), casual and a little urgent.
- **Do** put the Facebook link in exactly two places: as the outlined button next to "Text me for photos" in the work/photos section, and in the footer nav. Its icon is Facebook blue (`#1877f2`).
- **Do** add new animated scenes through `Loop.add` with a reduced-motion still frame.
- **Do** tune canvases through their tunables block.

### Don't:
- **Don't** add a sticky or fixed bottom call bar. The header number and in-flow buttons are the whole contact system.
- **Don't** show the phone number anywhere else on the first screen. On first view it lives top-right in the header only. It appears again only in the footer and in the form's fallback line.
- **Don't** add an email address, a contact form that posts to a server, hours, prices, reviews, a license or insurance claim, a company name, or photos. None of those exist yet. Gaps stay gaps.
- **Don't** add a webfont, a second typeface, or uppercase body copy.
- **Don't** add cards, a service-card grid, stock photography or tool icons. Services are rows, and the scenes are the imagery.
- **Don't** change the service row itself on hover or focus. Only the arrow responds.
- **Don't** use gold for focus on kraft or rust for focus on dark grounds.
- **Don't** add UI shadows beyond the filled-button lift.
