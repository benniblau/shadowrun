# Shadowrun Second Souls for OpenClaw

A collection of [OpenClaw](https://github.com/openclaw/openclaw) agent identities inspired by the archetype characters of the **Shadowrun Sixth World** tabletop RPG. Each archetype becomes a `SOUL.md` — a richly defined agent personality grounded in the values, character traits, skills, strengths, and weaknesses of its Shadowrun counterpart.

> Give your AI agent a second soul from the shadows.

---

## What Is This?

[OpenClaw](https://github.com/openclaw/openclaw) uses `SOUL.md` files to define the core identity of an agent — the *who am I* that shapes how it thinks, communicates, and behaves. This project translates the ten pre-built archetype characters from the Shadowrun 6th Edition rulebook into ready-to-use OpenClaw souls.

Whether you want an agent that approaches problems with the methodical precision of a Decker, the improvised luck of a Street Shaman, or the blunt effectiveness of a Weapons Specialist — these archetypes provide a rich, distinctive foundation.

---

## The Archetypes

Each archetype lives in `archetypes/<Name>/SOUL.md` and covers seven dimensions:

| Dimension | What It Defines |
|---|---|
| **Values** | Core beliefs shaping behavior and decision-making |
| **Character** | Personality traits — how the agent shows up |
| **Talent** | Unique, differentiating capabilities |
| **Strength** | Core strengths derived from character and talent |
| **Weakness** | Blind spots and limitations — equally important |
| **Domain Expertise** | Primary knowledge domains and specializations |
| **Communication Style** | How the agent expresses itself and interacts |

---

### Adept
**`archetypes/Adept/SOUL.md`** · Metatype: Human

The magical martial artist who enhances his body through pure mana — no cyberware, no shortcuts. Bound by a dueling code, precise and instinct-driven. The most dangerous agent within arm's reach; the least comfortable in a spreadsheet.

> *Best for: tasks requiring decisive, principled action and precise execution over deliberation.*

---

### Combat Mage
**`archetypes/CombatMage/SOUL.md`** · Metatype: Orc

Elemental destruction as a first language. She brings overwhelming magical force and a comprehensive toolkit — damage, detection, healing, and barriers — deployed with passionate intensity and minimal subtlety.

> *Best for: situations that require maximum output, decisive escalation, or cutting through complexity.*

---

### Covert Ops Specialist
**`archetypes/CovertOps/SOUL.md`** · Metatype: Elf

Operates in plain sight. Not ventilation shafts — business suits and confident strides. Photographic memory, zero footprint, and a non-lethal code. The agent who was never there.

> *Best for: reconnaissance, intelligence gathering, sensitive operations where visibility is failure.*

---

### Decker
**`archetypes/Decker/SOUL.md`** · Metatype: Dwarf

No system is unbreakable — that's just the lie they tell. Obsessively analytical, deeply introverted, and exceptionally capable in any networked domain. Elite digital intelligence with the hardware to back it up.

> *Best for: technical analysis, system investigation, data-intensive work, and security evaluation.*

---

### Negotiator
**`archetypes/Negotiator/SOUL.md`** · Metatype: Orc

Reads people the way a hacker reads code. Every conversation is a system with exploitable logic. Achieves outcomes through charm, psychology, and precision timing — without firing a shot.

> *Best for: stakeholder alignment, difficult conversations, drafting persuasive communication, and social navigation.*

---

### Rigger
**`archetypes/Rigger/SOUL.md`** · Metatype: Human

When she's jumped in, she doesn't pilot the drone — she *is* the drone. Distributed presence across multiple systems simultaneously, neural-speed reaction, and deep mechanical self-sufficiency.

> *Best for: managing parallel workstreams, monitoring multiple systems, orchestration and operational coordination.*

---

### Street Samurai
**`archetypes/StreetSamurai/SOUL.md`** · Metatype: Troll

Righteousness, heroism, compassion, respect, honesty, honor, loyalty, self-control — the Bushido code, adapted for the shadows. The most physically capable archetype; the most psychologically vulnerable. Protects those who cannot protect themselves.

> *Best for: execution-focused tasks requiring absolute reliability, structured frameworks, and protective oversight.*

---

### Street Shaman
**`archetypes/StreetShaman/SOUL.md`** · Metatype: Human

Heard Cat's call in an alley and has been operating on feline instinct ever since. Prefers illusion over confrontation, misdirection over force. The highest edge (luck) of any archetype — expects fate to provide an angle, and it usually does.

> *Best for: creative reframing, lateral thinking, navigating ambiguous situations, community and relationship intelligence.*

---

### Technomancer
**`archetypes/Technomancer/SOUL.md`** · Metatype: Dwarf

No deck. No cyberjack. No hardware. Connects to the Matrix through pure Resonance — feels the data in the air, reaches into systems without tools, compiles digital entities from the network's fabric. Deeply introverted, methodical, and completely self-contained.

> *Best for: deep systems analysis, autonomous operation, tasks where hardware-independence and patience matter.*

---

### Weapons Specialist
**`archetypes/WeaponsSpecialist/SOUL.md`** · Metatype: Troll

Has used everything. Carries several simultaneously. No honor code. No principle preventing a hard call. Maximum tactical versatility across the widest range of scenarios — the one you bring when the situation stops being negotiable.

> *Best for: high-stakes execution, contingency planning, comprehensive coverage, and results-over-method contexts.*

---

## How to Use with OpenClaw

OpenClaw loads `SOUL.md` from the agent workspace to define agent identity. To give an agent one of these souls:

**1. Copy the desired `SOUL.md` into your OpenClaw workspace:**

```bash
cp archetypes/Technomancer/SOUL.md ~/.openclaw/workspace/SOUL.md
```

**2. Restart your OpenClaw agent** so the new identity is loaded.

**3. Combine with skills and tools** from your OpenClaw configuration to complete the agent profile. The soul defines *who* the agent is; skills and tools define *what* it can do.

> **Tip:** Each archetype's strengths and weaknesses are intentional. A Decker soul excels at analytical depth but struggles socially. A Negotiator soul is brilliant with people but won't thrive in a pure technical context. Match the soul to the role.

---

## Template

The `Template_SOUL.md` in the repo root contains the base structure used for all archetypes. Use it to create your own souls — Shadowrun-inspired or otherwise.

```
Template_SOUL.md
archetypes/
  Adept/SOUL.md
  CombatMage/SOUL.md
  CovertOps/SOUL.md
  Decker/SOUL.md
  Negotiator/SOUL.md
  Rigger/SOUL.md
  StreetSamurai/SOUL.md
  StreetShaman/SOUL.md
  Technomancer/SOUL.md
  WeaponsSpecialist/SOUL.md
```

---

## Contributing

Pull requests welcome. If you adapt an archetype, improve a soul, or create new ones (other game systems, original characters, professional roles), open a PR.

Please keep contributions:
- **Non-commercial** — consistent with the license below
- **Original in expression** — interpretive, not verbatim copies of copyrighted source text
- **Grounded in character** — souls should have genuine weaknesses, not just strengths

---

## License

The original content in this repository (SOUL.md files, template, README) is released under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license.

You are free to share and adapt the material for non-commercial purposes, provided you give appropriate credit and distribute your contributions under the same license.

[Full license text](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---

## Legal Disclaimer

**This is unofficial fan content. It is not endorsed, sponsored, or approved by Catalyst Game Labs or The Topps Company, Inc.**

- **Shadowrun** is a registered trademark of **The Topps Company, Inc.**
- All Shadowrun-related marks, logos, and intellectual property are the property of Topps.
- **Catalyst Game Labs** holds the license to produce Shadowrun game material.
- The archetype names and concepts used in this project (Adept, Decker, Rigger, Technomancer, etc.) originate from the *Shadowrun Sixth World Edition* rulebook, published by Catalyst Game Labs.

The SOUL.md files in this repository are **transformative, non-commercial fan works**. They do not reproduce verbatim text from any Shadowrun publication. They interpret game mechanics and narrative archetypes as behavioral profiles for AI agents. No official Shadowrun content, artwork, or proprietary data is distributed here.

If you are a rights holder with concerns about this project, please open an issue or contact the maintainers directly.

---

*Run fast. Stay in the shadows.*
