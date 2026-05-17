# 05 3D Pipeline

## File Purpose

This file defines the professional 3D production workflow for the character.

The goal is to turn the approved concept and visual design bible into a controlled, game-ready character production plan.

This file focuses on process, order of work, quality gates, and dependencies.

It does not finalize technical specs such as polycount, UV layout, texture resolution, shader setup, or engine settings. Those will be defined later in `06_technical_specs.md`.

## Current Production Direction

Character direction:

Non-psyker, human-scale Ordo Malleus Inquisitor.

Approved visual foundation:

* Close Henry Cavill-inspired older veteran face, not direct commercial replica
* Bare head as primary presentation
* Mid-to-late 40s apparent age
* Strong but realistic human body
* Custom human-scale Inquisitorial power armor
* Long cloak over the armor
* Hood resting behind the head or on the upper back
* Possible tabard or controlled chain arrangement, pending visual exploration
* Human-scale pauldrons, armored bracers, armored gloves, and armored boots
* Controlled belt, holster, scabbard, and rosette zone
* One primary melee weapon: power sword
* One secondary sidearm: bolt pistol
* One optional relic maximum, pending decision
* Limited purity seals
* No books in v1
* No servo-skull in v1
* No helmet in v1
* No Space Marine backpack or power unit silhouette
* Standing authority pose

Main portfolio priorities:

1. Face and likeness quality
2. Full-body power armor silhouette
3. Power armor hard-surface construction
4. Cloak and hood integration
5. Material realism
6. Game-ready optimization
7. Clean final presentation

## Core Pipeline Rule

Do not start final sculpting or small detail work until the silhouette, proportions, costume layers, armor placement, and prop placement are approved.

Bad order:

Small details first, then fixing the body and silhouette later.

Correct order:

Foundation first, detail later.

## Recommended Software Stack

Primary tools:

* ZBrush for sculpting
* Marvelous Designer for cloak, hood, and possible tabard exploration
* Blender or Maya for power armor modeling, retopology, layout, and scene organization
* Substance 3D Painter for texturing
* Substance 3D Designer or Photoshop for custom material support, if needed
* Marmoset Toolbag or Unreal Engine for baking, lookdev, and final presentation
* PureRef or similar tool for reference boards

Optional tools:

* RizomUV for UVs
* ZWrap or Wrap for likeness/base mesh workflow, if available
* FiberShop, XGen, Blender curves, or Unreal groom workflow for hair and beard
* TopoGun, Maya Quad Draw, or Blender retopology tools

Use the tools that best support clean results. Do not change tools just because they are trendy.

## Folder Structure

Recommended working folder structure:

```text
project/
├── docs/
│   ├── 00_project_instructions.md
│   ├── 01_lore_research.md
│   ├── 02_reference_sources.md
│   ├── 03_character_concept.md
│   ├── 04_visual_design_bible.md
│   ├── 05_3d_pipeline.md
│   ├── 06_technical_specs.md
│   ├── 07_asset_checklist.md
│   ├── 08_decision_log.md
│   └── 09_feedback_log.md
│
├── references/
├── blockout/
├── sculpt/
│   ├── head/
│   ├── body/
│   ├── coat/
│   ├── armor/
│   ├── props/
│   └── weapons/
│
├── modeling/
├── retopo/
├── uvs/
├── baking/
├── textures/
├── groom/
├── rig_prep/
├── presentation/
│   ├── marmoset/
│   ├── unreal/
│   ├── renders/
│   └── breakdowns/
└── exports/
```

## Naming Convention

Use clear file names.

Recommended format:

```text
assetname_stage_version.ext
```

Examples:

```text
inquisitor_body_blockout_v001.blend
inquisitor_head_sculpt_v003.zpr
cloak_highpoly_v002.zpr
power_armor_chest_lowpoly_v001.fbx
power_sword_highpoly_v001.blend
rosette_texture_v002.spp
```

Rules:

* Never overwrite major milestones.
* Use version numbers.
* Keep exported files separate from working files.
* Keep blockout, high-poly, low-poly, UV, texture, and presentation files separate.

## Pipeline Overview

Recommended production order:

1. Reference board lock
2. Base body proportion blockout
3. Head likeness blockout
4. Power armor proportion blockout
5. Full-body silhouette blockout
6. Cloak and hood blockout
7. Optional tabard / controlled chain exploration
8. Belt, rosette, scabbard, holster, weapon, and relic placement
9. First full design review
10. Head and body high-poly sculpt
11. Power armor high-poly hard-surface modeling
12. Cloak, hood, and cloth high-poly construction
13. Weapons and props high-poly
14. Retopology
15. UV layout
16. Baking
17. Texturing
18. Grooming
19. Rig-ready cleanup
20. Lookdev
21. Final presentation
22. ArtStation breakdown

## Phase 1: Reference Board Lock

Purpose:

Before opening ZBrush or modeling software, collect and organize reference.

Required reference boards:

* Official Ordo Malleus / Inquisitor visual references
* Human-scale Inquisitor references
* Official Inquisitors in heavy armor / power armor references
* Human-scale power armor references
* Henry Cavill-inspired likeness references
* Cloak, hood, and tabard references
* Chain arrangement references, if explored
* Power armor hard-surface reference
* Negative Space Marine reference board
* Cloak, ceremonial cloth, and armor-over-cloth references
* Custom human-scale power armor and hard-surface reference
* Leather, cloth, wax, parchment, brass, and gunmetal material references
* Power sword and sidearm references
* Rosette and authority-object references
* Real-time character quality benchmark references
* Negative reference board

Quality gate:

Do not continue until references are separated by purpose and source category.

Do not use fan art as lore authority.

## Phase 2: Base Body Proportion Blockout

Purpose:

Establish the human-scale foundation.

Tasks:

* Build or import a neutral human base mesh
* Set height around 188-190 cm if approved in the visual bible
* Keep proportions strong but realistic
* Avoid Space Marine scale
* Check head-to-body ratio before adding costume
* Block broad shoulders without superhero exaggeration
* Build in a neutral A-pose or relaxed production pose
* Confirm body still reads as tall human after power armor volume is added
* Keep head size large enough to avoid Astartes proportions
* Reserve armor thickness without creating a barrel torso
* Check cloak length against final silhouette

Quality gate:

The body must read as a powerful human before armor is added.

Common mistakes:

* Head too small
* Shoulders too wide
* Hands too large
* Boots too oversized
* Body hidden too early by costume
* Power armor makes the head look too small
* Torso becomes too wide and barrel-shaped
* Boots become Space Marine-sized

## Phase 3: Head Likeness Blockout

Purpose:

Establish the hero asset early.

Tasks:

* Block skull shape first
* Build jaw, brow, cheekbones, nose, eyes, and mouth planes
* Use Henry Cavill-inspired reference, not a direct scan copy by default
* Keep apparent age in mid-to-late 40s
* Add beard and hair only after main forms work
* Test expression as calm, severe, and controlled

Quality gate:

The head must still work without costume, lighting tricks, or props.

Do not over-detail pores before likeness, planes, and expression are correct.

## Phase 4: Full-Body Silhouette Blockout

Purpose:

Test the character read from distance.

Tasks:

* Add rough power armor mass
* Add rough cloak volume
* Add hood resting behind the head or on the upper back
* Test possible tabard or controlled chain arrangement
* Add rough shoulder armor volume
* Add belt / authority zone
* Add power sword and bolt pistol positions
* Add boot mass
* Test from front, side, and three-quarter view
* Test with small thumbnail renders

Quality gate:

In three seconds, the character should read as:

* Human
* High-ranking
* Inquisitor in power armor
* Grimdark Imperial-style authority
* Daemon-hunter / forbidden-threat investigator
* Not Space Marine
* Not priest
* Not commissar
* Not fantasy knight

Do not continue to detail until this works.

## Phase 5: Costume Layer Blockout

Purpose:

Build believable construction.

Layer order:

1. Body base
2. Under-armor layer
3. Custom human-scale power armor
4. Long cloak
5. Hood resting behind the head or on the upper back
6. Optional tabard or controlled chain arrangement
7. Belt / authority system
8. Scabbard and holster
9. Armored gloves and boots
10. Rosette
11. Optional relic
12. Limited purity seals

Tasks:

* Check armor thickness
* Define power armor torso proportions
* Define shoulder width
* Define cloak length and attachment logic
* Define hood resting position
* Test tabard or controlled chain option if included
* Keep all cloth heavy and believable
* Avoid robe-like priest silhouette
* Avoid Space Marine silhouette

Quality gate:

The costume must look wearable, constructible, and human-scale.

No floating parts. No random panels. No detail without attachment logic.

## Phase 6: Armor Blockout

Purpose:

Make power armor readable, expensive, and imposing without turning the character into a Space Marine.

Approved v1 armor zones:

* Power armor chest and torso
* Human-scale pauldrons
* Bracers and armored gloves
* Thigh and knee armor
* Lower-leg armor
* Heavy armored boots
* Compact rear armor structure without backpack silhouette

Not approved for v1:

* Space Marine backpack
* Astartes-style power unit silhouette
* Full helmet
* Oversized pauldrons
* Barrel-shaped Space Marine torso
* Chapter markings
* Massive gorget or collar that hides the neck and jaw

Tasks:

* Fit armor over the body base
* Keep armor human-scale
* Check head-to-body ratio after armor mass is added
* Check shoulder width limit
* Maintain neck and jaw visibility
* Preserve cloak silhouette
* Keep trim restrained
* Ensure rear armor does not read as Space Marine backpack

Quality gate:

Armor must read as custom Inquisitorial power armor, not Astartes armor.

## Phase 7: Authority Zone, Weapon, And Prop Placement

Purpose:

Control the visual center of authority.

Tasks:

* Place rosette first
* Place power sword and scabbard
* Place bolt pistol and holster
* Add only necessary pouches or armor-mounted utility items
* Test optional relic only if it improves the concept
* Test tabard or controlled chain relationship to belt and armor
* Test front and three-quarter readability
* Check clipping with cloak, sword, pistol, and boots

Belt / authority cap:

* Rosette
* Bolt pistol holster
* Power sword scabbard
* Two small pouches maximum
* One relic attachment point only if relic is chosen
* Controlled chain arrangement only if it supports silhouette and does not create clutter

Quality gate:

The belt must feel functional and authoritative, not overloaded.

## Phase 8: First Full Design Review

Purpose:

Catch major problems before high-poly work.

Review checklist:

* Does the power armor silhouette work?
* Does the face remain the hero?
* Does the character read as human?
* Does the armor avoid Space Marine scale?
* Does the rear view avoid Space Marine backpack / power unit silhouette?
* Does the cloak improve the Inquisitor read?
* Is tabard or chain arrangement helping rather than cluttering?
* Is the belt / authority area overloaded?
* Are there too many seals, chains, or relics?
* Is the Ordo Malleus identity visible without clutter?
* Is the pose still calm and authoritative?
* Are any elements drifting toward priest, commissar, tech-priest, fantasy knight, or Space Marine?

If the answer is weak, fix it now.

Do not move to high-poly to “save” a bad blockout.

## Phase 9: High-Poly Sculpt And Modeling

Recommended order:

1. Head and facial structure
2. Body anatomy under armor
3. Power armor large forms
4. Power armor secondary hard-surface forms
5. Cloak and hood primary folds and construction
6. Optional tabard or controlled chain elements
7. Armored boots and gloves
8. Belt, holster, and scabbard
9. Weapons
10. Rosette
11. Optional relic
12. Purity seals
13. Surface damage and wear

Rules:

* Large forms first
* Secondary forms second
* Micro detail last
* Keep damage controlled
* Keep religious/gothic elements restrained
* Do not add new props during high-poly unless something else is removed
* Do not add Space Marine backpack logic during high-poly
* Do not let chain details replace strong armor forms
* Hard-surface bevels must be clean and bakeable

## Phase 10: Retopology

Purpose:

Create game-ready low-poly assets.

General approach:

* Retopologize by material and deformation needs
* Keep clean edge loops around face, eyes, mouth, neck, shoulders, elbows, wrists, hips, knees, and ankles
* Use separate meshes where it helps production and baking
* Keep armor and props efficient
* Avoid unnecessary hidden geometry
* Prepare clothing for possible rigging and posing
* Retopologize power armor as separate logical armor pieces where useful
* Keep cloak topology clean enough for final pose
* Avoid hidden geometry under cloak and armor
* Preserve armor silhouette edges efficiently

Important:

Final topology budget belongs in `06_technical_specs.md`.

This file only controls workflow.

## Phase 11: UV Layout

Purpose:

Prepare clean texture sets.

General approach:

* Group UVs by material and asset importance
* Give the face enough texel density
* Prioritize visible hero areas
* Keep shells clean and readable
* Avoid wasting texture space on hidden surfaces
* Plan separate texture sets only where justified

Possible texture set groups to decide later:

* Head / skin
* Hair / beard
* Under-armor layer
* Power armor
* Cloak / hood
* Tabard or chains, if approved
* Leather belt / holster / scabbard
* Weapons
* Rosette / relic / seals

Final texture set count belongs in `06_technical_specs.md`.

## Phase 12: Baking

Purpose:

Transfer high-poly detail cleanly to low-poly assets.

Bake maps likely needed:

* Normal
* Ambient occlusion
* Curvature
* Thickness if needed
* Position
* ID map
* Height if needed

Rules:

* Test bake early on one armor asset
* Fix cage issues before full baking
* Check seams
* Check hard edges
* Check projection errors
* Keep naming clean

Quality gate:

No major bake artifacts on face, power armor chest, shoulder armor, cloak edges, weapons, holster, scabbard, or rosette.

## Phase 13: Texturing

Purpose:

Create believable, controlled material storytelling.

Material priorities:

1. Skin and grooming
2. Power armor
3. Cloak and hood cloth
4. Leather and utility items
5. Gunmetal and tarnished brass / gold trim
6. Parchment and wax
7. Weapons
8. Rosette and optional relic
9. Optional tabard or controlled chains

Rules:

* Materials must look aged but maintained
* Wear must follow contact logic
* Dirt belongs in seams and lower areas
* Metal edge wear must be controlled
* Wax and parchment must not look like plastic
* No readable text until approved
* No random symbols
* Armor should look expensive, ceremonial, battle-used, and maintained.

Quality gate:

Each material should be identifiable without relying on labels.

## Phase 14: Grooming

Purpose:

Create realistic hair and beard that support the face.

Tasks:

* Build disciplined short-to-medium hair
* Build short beard or facial hair
* Add breakup and natural density variation
* Avoid perfect salon grooming
* Avoid messy fantasy barbarian hair
* Test in final lighting early

Groom method to decide in `06_technical_specs.md`.

Possible options:

* Hair cards
* Curve groom
* Unreal groom
* Marmoset-compatible hair setup

## Phase 15: Rig-Ready Preparation

Purpose:

Make the character usable for posing and presentation.

Tasks:

* Check mesh intersections
* Clean transforms
* Name meshes clearly
* Keep pivot points logical
* Prepare separate prop meshes
* Check cloak clearance against legs and boots
* Check armor intersections at shoulders, elbows, hips, knees, and ankles
* Check sword scabbard and pistol holster do not clip through cloak
* Check chains do not create impossible posing problems if chains are approved
* Check shoulder range
* Check hand-to-weapon relationship
* Prepare neutral pose and final hero pose

Rigging depth will be defined later.

Minimum requirement:

The model must support a clean standing authority pose.

## Phase 16: Lookdev And Presentation

Purpose:

Make the final character look portfolio-ready.

Presentation targets:

* Full-body hero render
* Front, side, and back turntable
* Face close-up
* Power armor close-ups
* Cloak / hood close-up
* Belt, rosette, weapon, scabbard, and holster close-up
* Material close-ups
* Wireframe or topology breakdown
* Texture flats
* Sculpt breakdown
* Optional tabard / chain exploration breakdown if used
* Optional fan-art vs safer original comparison, if needed

Primary pose:

Standing authority pose.

Recommended pose logic:

* Left hand near rosette, belt, or cloak edge
* Right hand relaxed or near sidearm
* Power sword sheathed or held low
* Face visible
* Cloak silhouette clear
* Power armor readable
* No combat pose as main render

Avoid:

* Combat pose as the main render
* Weapon blocking the face
* Overly dramatic superhero stance
* Excessive smoke, bloom, or effects hiding asset quality

## Quality Gates Summary

Do not move forward unless each gate is passed.

### Gate 1: Reference Gate

References are organized by source type and purpose.

### Gate 2: Proportion Gate

The body reads as a powerful human, not a Space Marine.

### Gate 3: Likeness Gate

The face has strong mature Cavill-inspired structure without becoming a direct commercial replica by default.

### Gate 4: Silhouette Gate

The character reads as a human-scale Inquisitor in power armor, not a Space Marine.

### Gate 5: Costume And Armor Gate

The power armor, cloak, hood, authority zone, and props are believable and constructible.

### Gate 6: Scope Gate

No extra weapons, books, relics, servo-skull, companion, helmet, Space Marine backpack, or diorama have entered v1.

### Gate 7: High-Poly Gate

Large and medium forms work before micro detail.

### Gate 8: Game-Ready Gate

Topology, UVs, bake, and textures support real-time presentation.

### Gate 9: Presentation Gate

Final renders clearly show face, silhouette, materials, topology, and production quality.

## Common Production Risks

### Risk 1: Overdecorating

Problem:

Too many seals, chains, skulls, relics, and inscriptions.

Control:

Use the prop cap and visual hierarchy.

### Risk 2: Space Marine Drift

Problem:

Shoulders, armor, and boots slowly grow too large.

Control:

Keep human proportions visible and compare against reference often.

* Check rear silhouette for backpack / power unit drift.
* Keep head size and human anatomy readable.
* Keep shoulders powerful but not Astartes-sized.

### Risk 3: Chain Overload

Problem:

Controlled chains can become visually impressive but may quickly create clutter, fantasy executioner language, or Chaos-adjacent read.

Control:

Use chains only if they improve silhouette and authority. Keep them secondary to face, power armor, cloak, and rosette.

### Risk 4: Losing The Face

Problem:

Armor, collar, weapon, or hood competes with the likeness.

Control:

Bare head remains primary. Neck and jaw must stay visible.

### Risk 5: Weak Lower Body

Problem:

Cloak dominates and legs feel unfinished.

Control:

Use strong armored boots and lower-leg armor logic.

### Risk 6: Fake Lore Detail

Problem:

Random symbols, fake text, or copied fan-art patterns.

Control:

No readable text or exact symbols until verified.

### Risk 7: Starting Detail Too Early

Problem:

Micro detail hides weak forms.

Control:

Pass silhouette and proportion gates first.

## Current Recommended Next Production Action

Before modeling begins, update:

`07_asset_checklist.md`

Reason:

The asset checklist must now reflect the approved power armor pivot, cloak, hood, power sword, bolt pistol, scabbard, holster, and pending tabard/chain exploration before blockout begins.

Recommended next design decision before blockout:

Torso silhouette exploration path.

Current recommendation:

Cloak plus short tabard and limited controlled chains.

Reason:

It preserves Inquisitorial ceremony while adding Ordo Malleus intimidation, without letting chains dominate the design.
