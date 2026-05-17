# 09 Feedback Log

## File Purpose

This file records project feedback, review notes, accepted fixes, rejected suggestions, deferred suggestions, and follow-up actions.

The goal is to keep feedback organized without letting review notes become scattered across chats, pasted text, or older project files.

This file is not the single source of truth for decisions.

Decision authority belongs to:

`08_decision_log.md`

If this file conflicts with `08_decision_log.md`, the decision log takes priority.

## Feedback Log Rules

1. Record important feedback here when it affects design, lore, scope, production, technical quality, or presentation.
2. Do not silently apply major feedback without logging it.
3. Use this file to track whether feedback was accepted, rejected, deferred, or needs more review.
4. If feedback changes a locked decision, update `08_decision_log.md` first.
5. If feedback requires edits to older files, list the affected files clearly.
6. Do not use this file as a place for random ideas or wishlist features.
7. Do not let feedback expand v1 scope unless something else is removed.
8. Feedback that adds props, symbols, inscriptions, weapons, or lore elements must be checked against lore and IP rules.
9. Once feedback is implemented, mark it as Integrated.
10. If feedback is useful but not for v1, mark it as Deferred to v2.

## Status Labels

Use these labels consistently:

* New
* Accepted
* Integrated
* Partially integrated
* Rejected
* Deferred to v2
* Needs lore verification
* Needs IP review
* Needs decision log update
* Needs file synchronization
* Superseded

## Feedback Categories

Use these categories:

* Lore accuracy
* Visual design
* Scope control
* Technical production
* Asset checklist
* Decision governance
* Reference management
* Presentation
* IP safety
* Production risk

## Feedback Entry Template

```text
Feedback ID:
Date:
Source:
Category:
Target file or area:
Feedback summary:
Recommendation:
Status:
Action taken:
Decision log impact:
Files updated:
Files still needing update:
Notes:
```

## Current Feedback Priorities

| Priority | Feedback Area | Status | Required Action |
|---:|---|---|---|
| 1 | Synchronize all project files with power armor pivot | Active | Confirm files 01, 03, 04, 05, 06, 07, 08, 09 are aligned |
| 2 | Pauldron shape | Pending decision | Explore compact, ceremonial, and hybrid human-scale options |
| 3 | Tabard versus controlled chain arrangement | Pending visual exploration | Test during silhouette concept pass |
| 4 | Rosette placement | Pending decision | Decide belt, chain, chest badge case, or revealable hidden placement |
| 5 | Optional relic | Pending decision | Decide none, warding reliquary, or sealed document case |
| 6 | Readable inscriptions | Pending decision | Keep no readable text unless verified and approved |
| 7 | Avoid documentation replacing production | Active risk | After synchronization, move into reference board and blockout |

## Integrated Feedback Log

### F001: Lock Ordo Direction

Date: 2026-05-16

Source: Review of `01_lore_research.md` and `03_character_concept.md`

Category: Lore accuracy / visual design

Target file or area:

* `01_lore_research.md`
* `03_character_concept.md`
* `04_visual_design_bible.md`
* `08_decision_log.md`

Feedback summary:

The character direction was too soft because Ordo Malleus and Ordo Hereticus were both still treated as possible final directions.

Recommendation:

Lock Ordo Malleus as the final direction. Keep Ordo Hereticus only as a secondary reference for severity and judicial restraint.

Status:

Integrated.

Action taken:

Ordo Malleus was locked as the final v1 Ordo direction.

Decision log impact:

Recorded as approved in `08_decision_log.md`.

Files updated:

* `01_lore_research.md`
* `03_character_concept.md`
* `04_visual_design_bible.md`
* `08_decision_log.md`

Files still needing update:

None known after synchronization.

Notes:

This prevents downstream prop and silhouette drift.

### F002: Replace “Mostly Puritan” Wording

Date: 2026-05-16

Source: Review of `03_character_concept.md`

Category: Lore accuracy

Target file or area:

* Puritan / Radical position

Feedback summary:

“Mostly Puritan” was imprecise because Puritan versus Radical is a philosophical position, not a simple decoration spectrum.

Recommendation:

Use “Puritan in philosophy, severe in method.”

Status:

Integrated.

Action taken:

The phrase was adopted as the official character philosophy.

Decision log impact:

Recorded as approved in `08_decision_log.md`.

Files updated:

* `01_lore_research.md`
* `03_character_concept.md`
* `04_visual_design_bible.md`
* `08_decision_log.md`

Notes:

This keeps the character morally severe without pushing him into Radical or Chaos-adjacent visual language.

### F003: Commit To Non-Psyker Direction

Date: 2026-05-16

Source: Concept review and user approval

Category: Lore accuracy / scope control / visual design

Target file or area:

* Psyker status

Feedback summary:

The character’s psyker status was open, which affected weapon logic, effects, eye treatment, and relic design.

Recommendation:

Lock him as a non-psyker Ordo Malleus Inquisitor with strict warding and relic discipline.

Status:

Integrated.

Action taken:

Non-psyker direction was approved and recorded.

Decision log impact:

Recorded as approved in `08_decision_log.md`.

Files updated:

* `04_visual_design_bible.md`
* `05_3d_pipeline.md`
* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This reduces fantasy effects and keeps the portfolio focus on face, armor, materials, and game-ready construction.

### F004: Lock Armor Over Coat Structure

Date: 2026-05-16

Source: Review of `03_character_concept.md` and `04_visual_design_bible.md`

Category: Visual design / technical production

Target file or area:

* Costume layers
* Armor placement

Feedback summary:

“Carapace under or over coat elements” was vague and would create different production paths.

Recommendation:

Lock carapace armor over a structured high-collar coat.

Status:

Superseded.

Action taken:

This was previously integrated, but it has now been superseded by the approved power armor pivot.

Decision log impact:

Superseded in `08_decision_log.md`.

Files updated:

* `08_decision_log.md`

Notes:

This is no longer the v1 armor direction.

### F005: Define Chest Cuirass Scope

Date: 2026-05-16

Source: Review of `04_visual_design_bible.md`

Category: Visual design / asset checklist

Target file or area:

* Chest armor

Feedback summary:

The chest plate description needed clearer limits.

Recommendation:

Use a front cuirass ending around the navel, with no full power-armor torso and no Space Marine chest proportions.

Status:

Superseded.

Action taken:

The cuirass direction was replaced by custom human-scale power armor.

Decision log impact:

Superseded in `08_decision_log.md`.

Files updated:

* `08_decision_log.md`
* `06_technical_specs.md`
* `07_asset_checklist.md`

Notes:

The anti-Space-Marine controls remain valid and were carried forward.

### F006: Lock Hood As V1 Construction, Not V1 Variant Render

Date: 2026-05-16

Source: Review of `04_visual_design_bible.md` and `07_asset_checklist.md`

Category: Visual design / scope control

Target file or area:

* Hood
* Cloak construction

Feedback summary:

The hood was ambiguous: present, optional, or variant-only.

Recommendation:

Model the hood in v1, resting behind the head or on the upper back. Defer hood-over-head presentation to v2.

Status:

Integrated.

Action taken:

The hood was included as part of cloak / upper-back cloth construction.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `04_visual_design_bible.md`
* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This preserves silhouette interest without hiding the face.

### F007: Add Hard Limits To Pauldrons

Date: 2026-05-16

Source: Review of `04_visual_design_bible.md`

Category: Visual design / scope control

Target file or area:

* Pauldrons
* Human-scale rule

Feedback summary:

“Broad but not huge” was too subjective and could drift toward Space Marine proportions.

Recommendation:

Use measurable limits and explicit human-scale checks.

Status:

Partially integrated.

Action taken:

Powerful but human-scale pauldrons are approved as a rule. Exact pauldron shape remains pending.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This is now one of the most important concept exploration decisions.

### F008: Add Boots And Gloves As Explicit Assets

Date: 2026-05-16

Source: Review of `07_asset_checklist.md` and `08_decision_log.md`

Category: Asset checklist / technical production

Target file or area:

* Boots
* Gloves

Feedback summary:

Boots and gloves appeared in material and production notes but were not explicit checklist assets.

Recommendation:

Add them as named assets.

Status:

Integrated.

Action taken:

Armored boots and gloves are explicit power armor assets.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

They are now critical anti-Space-Marine scale controls.

### F009: Add Eyes As Dedicated Technical Asset

Date: 2026-05-16

Source: Review of `06_technical_specs.md`, `07_asset_checklist.md`, and `08_decision_log.md`

Category: Technical production / face quality

Target file or area:

* Eyes
* Face shader

Feedback summary:

Eyes were not tracked as a distinct asset despite being critical to the close-up face read.

Recommendation:

Add a dedicated eye asset/spec with cornea, sclera, iris depth or parallax, catchlight, and subtle moisture.

Status:

Integrated.

Action taken:

Eye shader target was included in technical specs through head/skin priority.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

The eyes must support the likeness, not become stylized fantasy eyes.

### F010: Lock Power Sword As Primary Melee Weapon

Date: 2026-05-16

Source: Repeated review feedback and user confirmation

Category: Asset checklist / decision governance / visual design

Target file or area:

* Primary melee weapon

Feedback summary:

The power sword was repeatedly recommended and later accepted as the main weapon direction.

Recommendation:

Lock power sword as the v1 primary melee weapon and defer daemonhammer.

Status:

Integrated.

Action taken:

Power sword was locked as the approved primary melee weapon.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This supports authority, calm pose, and avoids weapon-dominant silhouette.

### F011: Lock Bolt Pistol As Secondary Sidearm

Date: 2026-05-16

Source: User confirmation and decision log update

Category: Asset checklist / decision governance

Target file or area:

* Secondary sidearm

Feedback summary:

The sidearm needed to be locked to prevent repeated deferrals.

Recommendation:

Lock bolt pistol as the v1 sidearm. Defer inferno pistol to v2 or alternate version.

Status:

Integrated.

Action taken:

Bolt pistol was locked as the approved v1 sidearm.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This reduces prop uncertainty and supports a grounded, recognizable weapon setup.

### F012: Add Power Sword Scabbard / Sheath

Date: 2026-05-16

Source: Review of `07_asset_checklist.md`

Category: Asset checklist / presentation

Target file or area:

* Power sword attachment
* Hero pose

Feedback summary:

If the sword is sheathed or held low in the hero render, the sheath/scabbard is a real asset.

Recommendation:

Add scabbard or sheath as a named asset.

Status:

Integrated.

Action taken:

Power sword scabbard/sheath was added to the asset checklist.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

The sheath must integrate with armor, belt, cloak, and pose logic.

### F013: Tighten Belt / Authority Cap

Date: 2026-05-16

Source: Review of visual bible and asset checklist

Category: Scope control / asset checklist

Target file or area:

* Belt
* Holster
* Scabbard
* Rosette
* Pouches
* Relic attachment

Feedback summary:

The belt and authority zone risked becoming overloaded.

Recommendation:

Use a strict cap and make optional items earn their place.

Status:

Integrated.

Action taken:

Belt / authority cap was tightened in asset checklist and decision log.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

The authority zone is not a storage rack.

### F014: Lock No Servo-Skull In V1

Date: 2026-05-16

Source: Review of concept, visual bible, and asset checklist

Category: Scope control

Target file or area:

* Servo-skull

Feedback summary:

Servo-skull remained optional too long despite being a separate companion asset.

Recommendation:

Exclude servo-skull from v1 and move it to v2 candidate assets.

Status:

Integrated.

Action taken:

Servo-skull was excluded from v1.

Decision log impact:

Recorded as deferred to v2 in `08_decision_log.md`.

Files updated:

* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This remains important after the power armor pivot.

### F015: Lock Marvelous Designer For Cloth

Date: 2026-05-16

Source: Review of pipeline and technical specs

Category: Technical production

Target file or area:

* Cloak
* Hood
* Possible tabard

Feedback summary:

Marvelous Designer was needed for believable major cloth construction.

Recommendation:

Use Marvelous Designer for cloak, hood, and possible tabard.

Status:

Integrated.

Action taken:

Marvelous Designer is now required for primary cloth elements.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `08_decision_log.md`

Notes:

Pattern files and cloth construction can become part of the final ArtStation breakdown.

### F016: Add Early Groom Test

Date: 2026-05-16

Source: Review of pipeline and technical specs

Category: Technical production / face quality

Target file or area:

* Head likeness
* Hair and beard

Feedback summary:

Final grooming was too late in the pipeline because the beard affects the jawline and likeness read.

Recommendation:

Add early rough hair/beard test during the head likeness stage.

Status:

Integrated.

Action taken:

Early groom test requirement was added.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `08_decision_log.md`

Notes:

The final groom still happens later, but the face must be tested with rough beard/hair early.

### F017: Manual Sculpt From Reference, No Celebrity Scan Base

Date: 2026-05-16

Source: Review of pipeline, technical specs, and decision log

Category: IP safety / technical production

Target file or area:

* Head likeness workflow

Feedback summary:

The likeness pipeline path needed to be decided.

Recommendation:

Use manual sculpt from reference, not celebrity scan or photogrammetry base.

Status:

Integrated.

Action taken:

Manual sculpt from reference was locked.

Decision log impact:

Recorded in `08_decision_log.md` with trade-off note.

Files updated:

* `08_decision_log.md`

Notes:

Trade-off: longer sculpt time, stronger IP safety, more portfolio-defensible as original work.

### F018: Technical Specs Tightening

Date: 2026-05-16

Source: Review of `06_technical_specs.md`

Category: Technical production

Target file or area:

* Polycount
* Texture sets
* Hair budget
* UVs
* Tangent space
* Power armor
* Cloak
* Power sword emissive

Feedback summary:

The technical specs needed to reflect power armor and updated game-ready scope.

Recommendation:

Update polycount, texture sets, armor plan, cloak plan, chain risk, and presentation outputs.

Status:

Integrated.

Action taken:

Technical specs were recreated for the power armor direction.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `08_decision_log.md`

Notes:

This improves the credibility of the “game-ready” claim after the armor pivot.

### F019: Add Presentation Budget And Deliverable Warning

Date: 2026-05-16

Source: Review of pipeline, technical specs, and asset checklist

Category: Presentation / production risk

Target file or area:

* Final renders
* Breakdown outputs

Feedback summary:

Presentation deliverables require real time and should not be treated as a quick final step.

Recommendation:

Reserve 20-30 hours for final lookdev, lighting, framing, export, and breakdown preparation.

Status:

Integrated.

Action taken:

Presentation time warning remains active.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

Weak presentation can make strong assets look average.

### F020: Create Decision Log To Stop Repeated Deferrals

Date: 2026-05-16

Source: Cross-file review after files 00-07

Category: Decision governance

Target file or area:

* All project files

Feedback summary:

The same decisions were repeatedly listed as pending across multiple files, creating document drift.

Recommendation:

Create `08_decision_log.md` as the single source of truth.

Status:

Integrated.

Action taken:

Decision log was created and later updated to close repeated-decision loops.

Decision log impact:

This feedback created the decision log itself.

Files updated:

* `08_decision_log.md`

Notes:

This remains the most important governance improvement.

### F021: Power Armor Pivot

Date: 2026-05-16

Source: User direction in chat

Category: Visual design / lore accuracy / scope control / technical production / decision governance

Target file or area:

* Full character direction
* Armor system
* Silhouette
* Asset checklist
* Technical specs
* Decision log

Feedback summary:

The user clarified that power armor is a core desired feature and should be part of the main version, not a later alternate concept.

Recommendation:

Approve custom human-scale Inquisitorial power armor as the main v1 armor direction. Preserve human scale, bare head, no Space Marine backpack / power unit silhouette, no helmet, and no Astartes proportions.

Status:

Integrated.

Action taken:

Power armor was made the main v1 armor direction. Carapace-over-coat was superseded.

Decision log impact:

Major revision recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`
* `09_feedback_log.md`

Files still needing update:

* Confirm `01_lore_research.md`, `03_character_concept.md`, `04_visual_design_bible.md`, and `05_3d_pipeline.md` are synchronized if not already edited.

Notes:

This is the largest design pivot so far. It should be treated as a deliberate v1 direction, not a temporary experiment.

### F022: No Power Unit / Backpack Silhouette

Date: 2026-05-16

Source: User clarification

Category: Visual design / scope control

Target file or area:

* Rear silhouette
* Power armor design

Feedback summary:

The user clarified that there should be no visible power unit / backpack silhouette.

Recommendation:

Do not include a Space Marine-style backpack or Astartes-style rear power unit. Use compact rear armor structure only.

Status:

Integrated.

Action taken:

No backpack / power unit silhouette was locked as a core rule.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This is essential to avoid Space Marine drift.

### F023: Cloak, Hood, Tabard, And Chain Exploration

Date: 2026-05-16

Source: User preference and design discussion

Category: Visual design / scope control

Target file or area:

* Cloak
* Hood
* Tabard
* Controlled chains

Feedback summary:

The user wants a long cloak and hood. The user is open to a tabard and also mentioned seeing a powerful chain-heavy alternative. The final choice should be made during concept exploration.

Recommendation:

Approve long cloak and hood. Keep tabard versus controlled chain arrangement pending visual exploration. Current working recommendation is cloak plus short tabard and limited controlled chains.

Status:

Partially integrated.

Action taken:

Cloak and hood were approved. Tabard/chains remain pending.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

Chains can be powerful but must avoid Chaos-adjacent or fantasy executioner read.

### F024: Books Excluded From V1

Date: 2026-05-16

Source: User clarification

Category: Asset checklist / scope control

Target file or area:

* Optional relic
* Prop list

Feedback summary:

The user clearly stated that books are not needed.

Recommendation:

Exclude relic books / chained tomes from v1.

Status:

Integrated.

Action taken:

Books were excluded from v1. Optional relic options are now none, warding reliquary, or sealed document case.

Decision log impact:

Recorded in `08_decision_log.md`.

Files updated:

* `07_asset_checklist.md`
* `08_decision_log.md`

Notes:

This reduces clutter and avoids text problems.

## Active Feedback Items Not Fully Closed

### AF001: Synchronize Older Files With Power Armor Direction

Status:

Needs verification.

Issue:

Files 01, 03, 04, and 05 may still contain older carapace-over-coat language unless already edited.

Required action:

Confirm all files are synchronized with the power armor decision log.

Priority:

High.

Do before:

Reference board lock and blockout.

### AF002: Pauldron Shape Still Pending

Status:

Pending decision.

Issue:

Pauldrons are essential to power armor identity but can easily cause Space Marine drift.

Options:

* Compact human-scale
* Wider ceremonial
* Hybrid

Current recommendation:

Explore hybrid: powerful and ceremonial, but clearly human-scale.

Required action:

Decide during armor silhouette blockout.

Priority:

High.

### AF003: Tabard Versus Controlled Chains Still Pending

Status:

Pending visual exploration.

Issue:

The user likes both tabard and chain-heavy visual logic but wants to decide through concept exploration.

Options:

* Cloak plus front/back tabard
* Cloak plus controlled chain arrangement
* Cloak plus short tabard and limited controlled chains

Current recommendation:

Cloak plus short tabard and limited controlled chains.

Priority:

High.

### AF004: Rosette Placement Still Pending

Status:

Pending decision.

Issue:

Rosette is mandatory, but placement is not locked.

Options:

* Belt
* Chain
* Small chest badge case
* Partly hidden and revealable in presentation

Current recommendation:

Small chest badge case or chain placement for power armor direction.

Priority:

High.

### AF005: Optional Relic Still Pending

Status:

Pending decision.

Issue:

Optional relic is allowed but not required.

Options:

* No relic
* Warding reliquary
* Sealed document case

Current recommendation:

No relic unless the silhouette needs stronger Ordo Malleus read. Warding reliquary is the best optional choice if needed.

Priority:

Medium-high.

### AF006: Readable Inscriptions Still Pending

Status:

Pending / needs lore verification.

Issue:

Readable text remains risky because fake Latin, fake High Gothic, and copied text are not allowed.

Current recommendation:

No readable text in v1. Use blank or unreadable texture detail only.

Priority:

Medium.

### AF007: Final Output Specs Still Pending

Status:

Pending technical decision.

Issue:

Final render resolution, image format, and turntable/video specs are not fully locked.

Current recommendation:

Define before final lookdev.

Priority:

Medium.

### AF008: Documentation May Become A Substitute For Production

Status:

Active production risk.

Issue:

The documentation is now mature enough to build from. Continuing to refine documents without moving into reference collection and blockout may slow production.

Current recommendation:

After one synchronization pass, begin reference collection and body/power armor/cloak blockout.

Priority:

High.

## Rejected Or Deferred Feedback

### RF001: Servo-Skull In V1

Status:

Deferred to v2.

Reason:

Lore-appropriate, but it becomes a separate companion asset and increases scope.

### RF002: Daemonhammer As V1 Primary Weapon

Status:

Deferred to v2.

Reason:

Lore-appropriate for Ordo Malleus, but risks overpowering the silhouette and making the character weapon-dominated.

### RF003: Bionic Eye In V1

Status:

Deferred to v2.

Reason:

Could add story, but competes with the Cavill-inspired face and increases shader/detail work.

### RF004: Wide-Brimmed Hat In V1

Status:

Rejected for v1.

Reason:

Strong Inquisitor signal, but competes with face and changes the silhouette too much.

### RF005: Carapace-Over-Coat As Main V1 Armor Direction

Status:

Superseded.

Reason:

The user clarified that power armor is a core desired feature for the main character.

### RF006: Books / Relic Tome In V1

Status:

Rejected for v1.

Reason:

User does not want books in v1. Also reduces text and clutter risks.

## Feedback Source Summary

| Source Area | Main Value | Current Status |
|---|---|---|
| Concept file reviews | Locked Ordo, philosophy, head presentation, prop cap | Integrated |
| User power armor clarification | Pivoted v1 direction to custom human-scale power armor | Integrated |
| Visual bible reviews | Tightened silhouette, cloak, hood, pauldron risks, chain risk | Partially integrated |
| Pipeline reviews | Updated production order around armor, cloak, and authority zone | Needs verification in file 05 |
| Technical specs reviews | Updated polycount, UV, texture, armor, cloth, and presentation rules | Integrated |
| Asset checklist reviews | Rebuilt scope around power armor, cloak, weapons, and pending chains/tabard | Integrated |
| Decision log reviews | Created governance and recorded power armor pivot | Integrated |

## File Synchronization Checklist

Use this checklist after updating `08_decision_log.md`.

### Files To Check

* `01_lore_research.md`
* `03_character_concept.md`
* `04_visual_design_bible.md`
* `05_3d_pipeline.md`
* `06_technical_specs.md`
* `07_asset_checklist.md`
* `08_decision_log.md`
* `09_feedback_log.md`

### Decisions To Synchronize

* Power armor locked as main v1 direction
* Carapace-over-coat superseded
* No Space Marine backpack / power unit silhouette
* Long cloak approved
* Hood approved, resting behind head or upper back
* Tabard versus controlled chains pending
* Power sword locked as primary melee weapon
* Bolt pistol locked as secondary sidearm
* Daemonhammer deferred to v2
* Inferno pistol deferred to v2
* Books excluded from v1
* Henry Cavill-inspired, older veteran, not direct commercial replica
* Natural eyes, no bionic eye in v1
* No helmet in v1
* No servo-skull in v1
* Purity seals approved with 3-5 cluster cap
* Rosette placement still pending
* Optional relic still pending
* No readable inscriptions unless verified and approved
* Safer original symbol treatment preferred, final handling pending

### Synchronization Rule

Do not rewrite older files completely unless the user explicitly asks.

Only update the sections that conflict with `08_decision_log.md`.

## Next Recommended Action

Recommended next action:

Confirm files `01` to `09` are synchronized after the power armor pivot.

After synchronization:

Begin production preparation:

1. Collect reference boards for power armor, Coteaz, human-scale Inquisitors, cloaks, hoods, tabards, chains, materials, Cavill likeness, and negative Space Marine examples.
2. Explore three torso silhouette options.
3. Start base body, power armor, and cloak blockout.

## Working Principle

Feedback should improve the project, not expand it endlessly.

When feedback creates a new idea, ask:

1. Does it improve lore accuracy?
2. Does it improve visual clarity?
3. Does it improve production quality?
4. Does it fit v1 scope?
5. Does it avoid IP and symbol problems?
6. Does it move the project closer to blockout?

If the answer is no, defer it or reject it.
