---
title: Scrying
date created: 2026-04-17
last modified: 2026-04-17
Claude model: claude-opus-4-6
---

# Scrying

**Summary**: A 5th-level divination spell that allows remote observation of a creature or location. The central information security threat that [[green-slaad-enterprises]]'s [[information-security]] practice defends against.

**Sources**: raw/scrying.md, raw/Do The Players Know They Are The Target of Scry?.md, gse-site/information-security.md, gse-site/post-divination.md

**Last updated**: 2026-04-17

## Spell mechanics

- **Level**: 5th
- **School**: Divination
- **Casting time**: 10 minutes
- **Duration**: Concentration, 10 minutes
- **Range**: Self (sensor appears near target)
- **Save**: Wisdom

The caster can see and hear a creature on the same plane of existence. The target makes a Wisdom saving throw, modified by the caster's familiarity and any physical connection to the target:

| Knowledge level | Modifier |
|---|---|
| Secondhand (heard of target) | +5 |
| Firsthand (met target) | +0 |
| Extensive (know target well) | -5 |

| Physical connection | Modifier |
|---|---|
| Picture or likeness | -2 |
| Garment or possession | -4 |
| Body part, hair, or nail | -10 |

On a successful save, the target is unaffected and immune for 24 hours. On failure, an invisible, intangible sensor appears within 10 feet of the target, moving with them. The sensor appears as a luminous orb (about fist-sized) to anything that can see invisible objects. (source: raw/scrying.md)

The target does not know what they are saving against — only that they feel uneasy. A target who knows the spell is being cast can choose to fail the save. (source: raw/scrying.md)

## Detection

The sensor is invisible by default. It can be detected by:

- **See Invisibility** or **True Sight** — sensor appears as a luminous orb
- **Detect Magic** — shows divination magic in use (but requires ability to see invisible objects to locate the sensor)
- **Faerie Fire** — could incidentally reveal the sensor during combat

The community consensus is that targets do not automatically know they are being scried upon. The spell is designed for covert observation. Characters only become aware through active detection methods. (source: raw/Do The Players Know They Are The Target of Scry?.md)

## As a security threat

GSE's counter-scrying sweeps find approximately one active scrying effect per wizard per month. This rate has been stable — neither increasing nor decreasing. (source: gse-site/information-security.md)

Scrying becomes increasingly difficult to resist as the caster gains better information about the target. With extensive knowledge (-5) and a body part (-10), the save modifier reaches -15, making resistance nearly impossible for most targets. The practical implication: wizards must protect personal items and information about themselves to maintain any defense against scrying. (source: raw/scrying.md, raw/Do The Players Know They Are The Target of Scry?.md)

GSE's [[information-security]] practice addresses scrying through:

- Counter-scrying audits (sweeping for active divinations)
- Supply-chain inspection (preventing sympathetic links in components)
- Apprentice training (preventing schedule and location leaks that enable targeting)
- Warded communications (preventing identity spoofing that could facilitate targeting)

(source: gse-site/information-security.md)

## Scrying vs. physical security

GSE explicitly argues that scrying and divination cannot substitute for [[physical-security]]. Key limitations:

- Divination answers questions the wizard thought to ask — it does not detect unanticipated threats.
- Divination does not run continuously while the wizard sleeps.
- Divination operates on the wrong timescale to counter in-progress attacks.
- Divination provides knowledge but not attention — security is primarily an attention problem.

"The thing that gets a wizard killed is almost never the thing they asked about. It's the thing they would have asked about if only they had known to." (source: gse-site/post-divination.md)

## Community discussion on handling scrying

The Reddit thread documents DM approaches to managing scrying in play. Key perspectives:

- **Secret rolls preferred**: Most recommend the DM roll saves secretly or ask players to pre-roll d20s at session start, to prevent metagaming. (source: raw/Do The Players Know They Are The Target of Scry?.md)
- **Suspense vs. surprise debate**: Some DMs prefer openly telling players they're being scried to create tension ("someone is watching — who?"), citing Hitchcock's suspense vs. surprise theory. (source: raw/Do The Players Know They Are The Target of Scry?.md)
- **Frequency increases with tier**: Scrying becomes common at tier 2 and very common at tier 3. As adventurers gain fame, poorly targeted scries begin, improving as adversaries gain better information. (source: raw/Do The Players Know They Are The Target of Scry?.md)

## Related pages

- [[information-security]]
- [[physical-security]]
- [[green-slaad-enterprises]]
- [[halric-bren]]
