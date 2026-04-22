---
title: Detecting Scrying In Your Own Sanctum
date created: 2026-04-20
size: teach-small
type: new
answers questions: Q37, Q14
Claude model: claude-opus-4-7
---

## Brief: Detecting Scrying In Your Own Sanctum

**Answers questions from questions.md:** Q37 (sanctum-resident detection), and extends Q14 (general "can a target detect being scried" — answered at a spell-mechanic level, not a sanctum-design level).

**Size / type:** Teach-small · New stuff. The [[scrying]] wiki page and the [[information-security]] page both cover detection as a service GSE performs *to* a wizard; neither teaches what the wizard can build *into their own space*.

## Reader

A working practitioner who owns and controls their workspace — tower, cottage, sanctum, lab. Not adventurers, not travelers. Specifically: someone who reads GSE's counter-scrying numbers (roughly one active scry per wizard per month), doesn't want to pay for monthly sweeps, and wants the sanctum itself to notice.

[[iolanthe-marsk]] is the archetype on the budget side. [[halric-bren]] is the archetype on the "I'm already being targeted" side.

## Concrete problem manifestations

- You've read that See Invisibility reveals the sensor, but you're not going to walk around your own tower casting it every hour.
- You keep a locked component cabinet. You have no way to know if it's being observed while you open it.
- A client sent you a sealed brief last week. You read it at your desk. Nothing felt wrong. You have no way to know whether anything was wrong.
- You're about to take a meeting you don't want scried. Casting Detect Magic in front of the guest is rude and tips your hand if the source is the guest.

## Brand-agnostic teaching (biggest part)

Organize around the shift from *cast-on-demand* to *resident-and-scheduled*. The sanctum is the one place a wizard can pre-install detection; teach that advantage.

**What the sensor actually is.** An invisible, fist-sized luminous orb within 10 feet of the target, moving with them. Not a camera on a wall — a thing that follows you room-to-room. The implication for sanctum design: if a sensor is in the building, it is wherever *you* are in the building. Detection has to be where you are, not where the doors are.

**The three off-the-shelf detection tools, and what each is actually good for:**

- **See Invisibility** — lets you watch for the orb directly. Best built into a "check window" — a glyph on a single item (a ring, a reading lens) you activate only when you need to look. Keeps you from burning the spell slot on a full-room sweep.
- **True Sight** — stronger and more expensive. Reserved for the room where sensitive work happens (reading room, correspondence desk). Not for the whole tower.
- **Detect Magic** — tells you divination magic is present, not where. Best as the *first* layer (a trigger), paired with See Invisibility as the *second* layer (the locator).

**Make at least one of them resident, not cast-on-demand.** A few patterns:

- *The channelled Detect Magic font.* A scrying-style basin keyed to show divination auras at arm's length. Walk past it when you enter your work area. If the needle moves, you know before you sit down.
- *The Alarm-variant divination trigger.* A standard Alarm spell rewired to fire on divination-school magic crossing the ward line, not on physical intrusion. Audible inside only; a bell, not a shout. Covers the entry moment.
- *The scheduled sweep.* Not a spell — a habit. Same two-minute ritual every morning, same second one before any sensitive reading. Written into the day like locking the front door. Free. Works without any glyph work at all.

**The decoy trick.** Leave an obviously-interesting document open on your desk (a fake research note, a fake client ledger). A scrying sensor will position itself to read it. If a trusted apprentice or housekeeper sweeps that specific spot with See Invisibility once a day — or if you've set a pressure-pad glyph under the "decoy desk" that fires on any divination signature within 10 feet of it — the sensor outs itself by doing what a sensor does.

**What to do when you detect one.** Don't react visibly. Don't speak. The caster is watching and listening in real time — panic confirms you have something worth watching. Step out of the sensor's 10-foot radius by leaving the room. Route any sensitive conversation elsewhere. Start source-hunting separately — who knew you'd be here, who has a component of yours, who gains from watching.

**The honest limit.** Detection is not prevention. A caster with extensive knowledge of you and a body-part component has a −15 save modifier. You are not going to win that save. What detection buys is *notice* — you find out you're being watched, you can control what happens in the sensor's presence, and you can begin the investigation. Counter-scrying sweeps, warded rooms, and component hygiene are the prevention half; this piece is explicitly the detection half.

**What not to bother with.** Wall-mounted anti-scrying tapestries sold at market fairs. Blanket "anti-divination" wards around the whole property — expensive, fragile, and they make the scryer work harder, not give up. A single warded reading room is worth more than a weakly warded building.

## Where GSE fits (light)

Trailing footer, not integrated. Two lines:

- Sera Oak ([[sera-oak]]) will install a resident Detect Magic font or a divination-keyed Alarm variant as a one-off install, outside the retainer model, if a solo wizard wants the infrastructure without the monthly relationship.
- If the detection patterns above start firing and you want a source investigation, that's what the counter-scrying sweep is for. (source: `gse-site/information-security.md`)

No hard CTA. The piece should work for a reader who never contacts GSE.

## Frictionless CTA

A one-page printable: **"The Five-Minute Sanctum Scry Check."** The morning-ritual version of the scheduled sweep, condensed. No email gate, no form. Link at the end of the post, also available standalone on the site. If a reader takes nothing else from the piece, they take the checklist and do it.

## Experts to interview

- **Sera Oak** — GSE's infosec lead. Owns the counter-scrying practice; knows what actually works in an installed setup vs. what sounds good in theory. Primary source for the resident-vs-cast-on-demand distinction.
- **Halric Bren** ([[halric-bren]]) — current infosec retainer client who was actively targeted (the spoofed-sending incident). Useful for "what it felt like before I knew" color, if he's willing to be on the record.
- Optional: **Mirella Thane** ([[mirella-thane]]) for one quote on why detection matters for PR — a scry caught early changes what the adversary *can* use against you publicly, and that changes the crisis shape.

## Sources

- `wiki/scrying.md` (spell mechanics, existing detection methods, counter-scrying sweep rate)
- `raw/scrying.md` (D&D Beyond reference — sensor properties, save modifiers)
- `raw/Do The Players Know They Are The Target of Scry?.md` (community consensus that targets don't automatically know)
- `raw/gse-site/information-security.md` (counter-scrying audits, supply-chain inspection, the one-scry-per-wizard-per-month figure)
- `raw/gse-site/post-divination.md` (the "divination answers questions the wizard thought to ask" frame — useful for the honest-limit section)
- `raw/gse-calls/call-03-customer-infosec-halric.md` (Sera's working voice)
- `wiki/information-security.md`, `wiki/halric-bren.md`, `wiki/sera-oak.md`

## What to avoid

- Jargon (sympathetic linkage, divination-school resonance) without a plain-language gloss.
- Pretending detection prevents scrying. It doesn't. Say so early.
- Listicle compression — "5 ways to detect a scry!" flattens the resident-vs-on-demand distinction, which is the actual teaching.
- A fear frame. The rate is one per month on average; the piece should read as hygiene, not alarm.
- Burying the checklist CTA inside the post. It goes at the end, and it stands alone.
