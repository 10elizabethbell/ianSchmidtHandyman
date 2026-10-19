# Ian Schmidt — handoff at ~60%

**Live:** https://10elizabethbell.github.io/ianSchmidtHandyman/ · **Repo:** https://github.com/10elizabethbell/ianSchmidtHandyman · **Built:** 2026-10-19 from Muse brief of 2026-10-19 (two Facebook group ads, "Ocean county small businesses and services.")

## What's built
- One page, `index.html` (~45KB, no images to download). Phone first; checked at 360/390/414/430 in WebKit and Chrome, and 1440 desktop.
- World: "leaves now, lights next", his two seasonal ads. Pine-green ground, a lawn with a mulch-bed edge, leaf-bag kraft for reading sections, a night roofline for the lights.
- Signature element: the hero is a lawn covered in fallen maple, oak and elm leaves. Drag a finger (any direction) or move the mouse to rake them; they tumble, pile up and get blown off, and new leaves drift down to fill the gaps. When nobody's touching it, wind gusts sweep across. The same lawn comes back as a strip above the footer.
- Holiday lights: a string of C9 bulbs hanging from a shingled roof edge; they sway on their own, swing when a finger or mouse passes, and swing and brighten when tapped.
- Sections: header (name, "Yard work & handyman · Toms River", 732-300-4510 top right) → hero "Consider it handled." (his line) + Text for a free estimate / Pick what you need → services (8 rows, each opens a pre-written text naming the job) → holiday lights → "You deal with me" + 3 steps → "Want to see my work?" (text for before/after photos + Facebook) → estimate form ("Fall spots are filling up fast", his line) → footer.
- Contact: everything goes to `sms:+17323004510` with a pre-filled body. The form builds "Hi Ian, I'd like a free estimate. What: … Where: … notes, - name", opens Messages, and shows the message with a Copy button and the number as a fallback.

## Assumptions I made
- **Name:** no business name exists, so the site is "Ian Schmidt" (his own name, how he advertises). The brief says don't invent one. If he has a name, it goes in the header, footer, title and og tags.
- **Favicon / home-screen icon:** no logo, so an "IS" monogram in the site's lettering on pine with a rust bar. The header uses a small maple-leaf mark.
- **Colors:** none published; taken from the work (lawn, fall leaves, leaf-bag kraft, light-bulb gold).
- **Lights area:** the lights ad names no area; I assumed Toms River like the handyman ad.
- **Copy I wrote in his voice** (check with him): "I'll take care of it like it's my own, at a fair price I tell you up front."; "Text me and you get me. I'm the one who shows up and does the job, and I treat your yard and your house the way I'd want someone to treat mine."; step 3 "Your yard's back to looking like yours."; "I'll text you before-and-after photos of my work." (from his "Before-and-after photos available on request"). His own lines used verbatim: "Consider it handled.", "Fair, upfront pricing.", "for a fair price", "Fall spots are filling up fast", "Don't wait until the leaves bury your lawn". The Impeccable sweep cut "I do the work myself" because the brief doesn't say he works alone.
- **Service grouping:** "Yard" and "Around the house", and the short names (e.g. "Small home repairs" for "Small home repairs & general handyman work").
- **Audience:** not flagged 40+, so it has full motion. Toms River skews older; if Ellie or Ian says the customers are mostly retirees, switch to the still version (`older-audience.md`).

## Placeholders and gaps
- No photos of his work, so no proof section with pictures. The "Want to see my work?" section asks people to text for before/afters instead.
- No reviews, prices, hours, email, license or insurance. Nothing about them on the page.
- Facebook link is his **personal profile** (`profile.php?id=100015585766678`). Ask him whether he wants it linked, or if he makes a business page.

## Questions for the owner
- Do you have a business name (or want one on the site)?
- Can you send 6–10 photos, especially before/after pairs (leaf cleanups, mulch beds, trimmed shrubs, a hauled-out garage, lights at night)?
- Which towns do you cover past Toms River (Brick, Lakewood, Berkeley, Island Heights, Seaside…)?
- Do you take lights down after the holiday too? Do you supply the lights or hang the customer's?
- Any reviews from customers you'd want quoted?
- Okay to link your personal Facebook?

## Ideas not built (yours to pick)
- **Runner-up world:** the lights as the hero, a house roofline at dusk you "plug in" bulb by bulb with your finger. Strong from November on; could swap in seasonally (leaf hero until Thanksgiving, lights hero after).
- Other worlds considered: hauling (a truck bed you load with junk), mulch beds and trimmed shrubs, a workbench pegboard, mowing stripes.
- When photos arrive: before/after sliders with a plain divider beside the services, and "Click to see more of my work." with the Facebook link right under them.
- Little reward: a leaf-pile "crunch" bounce when you rake a big pile together.
- Lights section: a Christmas / Halloween / Thanksgiving switch that recolors the bulbs (red-green, orange-purple, amber).
- Seasonal headline swap in December: "Lights up. Consider it handled."

## Not verified
- Real-device touch on iPhone and Android, and inside Facebook's in-app browser (tested in desktop WebKit/Chrome with simulated touch).
- The real SMS handoff on iOS and Android (link format `sms:+1…?&body=` decodes correctly in tests).
- Frame rate on older phones (phone draws up to ~520 leaves; lower `MAX_LEAVES` at the top of the leaves script if it stutters).

## How it was checked
- Phone audit scripted in WebKit and Chrome at 360/390/414/430: no sideways overflow, all tap targets 44px+, inputs 17px (no iOS zoom), phone number 16px from the edge, text button on the first screen, all 11 pre-written texts decode, form errors and composed message correct.
- Motion: two frames differ; a simulated touch drag rakes up, down and sideways; a lights tap runs without errors.
- Impeccable: every mode except `live` (`onboard` didn't apply), plus the finish reviewer ("fix and ship"). Applied: header fit at 360, copy de-duplication and first-person fixes, denser lawn, shingled roof edge, tap-to-swing lights, rust focus ring on kraft, form `aria-describedby`/`aria-invalid`, chips in static HTML, copy-button reset, batched grass drawing. Not applied: leaves drifting behind the hero headline on desktop (house rule: nothing runs through text).
- Detector ignores added in `.impeccable/config.json`: `overused-font roboto` (system stack's Android fallback) and `cramped-padding` for index.html (the footer lawn strip is flush by design), plus `flat-type-hierarchy` and `tight-leading` scoped to index.html (the headings carry the hierarchy). After DESIGN.md landed, its drift findings were fixed by adding the missing tokens; the detector reports 0 findings.
