# 06 Technical Specs

## File Purpose

This file defines the technical production targets for the game-ready Inquisitor character.

The goal is to convert the approved concept, visual design bible, and 3D pipeline into practical production limits for modeling, retopology, UVs, baking, texturing, grooming, rig preparation, and final presentation.

This file controls:

* Scale and units
* Target renderer
* Polycount ranges
* Texture set plan
* UV strategy
* Bake requirements
* Material and shader plan
* Hair and beard method
* Cloth workflow
* Power armor workflow
* Rig and pose requirements
* Export formats
* Presentation technical targets
* Remaining technical decisions

## Technical Status

Current status: revised working technical target.

These specs are strong enough to guide production, but final numbers should be locked only after reference collection, silhouette blockout, armor blockout, cloak/tabard/chain exploration, and asset checklist approval.

## Current Character Inputs

Locked design direction:

* Character type: human-scale Ordo Malleus Inquisitor
* Philosophy: Puritan in philosophy, severe in method
* Psyker status: non-psyker
* Head presentation: bare head as primary
* Face direction: close Henry Cavill-inspired older veteran face, not direct commercial replica
* Age read: mid-to-late 40s
* Body scale: tall, strong human, not Space Marine
* Armor: custom human-scale Inquisitorial power armor
* Cloak: long cloak over armor
* Hood: present, resting behind the head or on the upper back
* Tabard / chain arrangement: pending visual exploration
* Primary melee weapon: power sword
* Secondary sidearm: bolt pistol
* Books: not included in v1
* Servo-skull: not included in v1
* Helmet: not included in v1
* Space Marine backpack / power unit silhouette: not allowed
* Pose: calm standing authority pose
* Primary renderer: Marmoset Toolbag for v1 presentation
* Unreal Engine: optional secondary presentation only

## Scale And Units

Working unit system:

* Centimeters
* Real-world scale
* Character height target: 188-190 cm

Scale rules:

* Body must remain believable as a tall human.
* Power armor must enhance authority without creating Astartes proportions.
* Head size must remain large enough to avoid Space Marine read.
* Hands, boots, pauldrons, and weapons must stay human-usable.
* Props must be measured against the body, not tabletop exaggeration.
* Rear silhouette must not create a Space Marine backpack or power unit read.

Recommended neutral production pose:

* Relaxed A-pose or relaxed T-pose during production
* Final posed version created later for presentation

Final presentation pose:

* Standing authority pose
* Left hand near rosette, belt, cloak edge, or sword hilt
* Right hand relaxed or near bolt pistol
* Power sword sheathed or held low
* Face clearly visible
* Cloak and power armor readable

## Target Renderer

Primary v1 target:

Marmoset Toolbag.

Reason:

Marmoset is efficient for high-quality character portfolio presentation, fast lookdev, baking checks, material review, turntables, and breakdown renders.

Unreal Engine status:

Optional secondary presentation only.

Warning:

Do not build final lookdev in both Marmoset and Unreal at the same time. Materials, lighting, exposure, and hair setup do not transfer perfectly. If Unreal is added later, allow extra time for material conversion and relighting.

## Game-Ready Target

The character should be game-ready for a high-end real-time portfolio, not a low-spec mobile asset.

Target category:

* Cinematic real-time hero character
* ArtStation portfolio quality
* Suitable for Marmoset or Unreal presentation
* Optimized enough to demonstrate professional game workflow

This is not intended as:

* A film-only sculpt
* A 3D-print miniature
* A mobile game asset
* A raw high-poly render only
* A non-optimized fan model

## Polycount Target

Final LOD0 target range:

* 220,000-320,000 triangles total, including hair cards and cloak

Preferred target:

* Around 260,000-280,000 triangles total if the silhouette and close-up quality justify it

Suggested allocation:

| Asset Area | Target Triangle Range |
|---|---:|
| Head and visible skin | 25,000-40,000 |
| Body under armor | 10,000-20,000 |
| Under-armor layer | 10,000-20,000 |
| Power armor set | 70,000-110,000 |
| Cloak and hood | 35,000-60,000 |
| Optional tabard / chains | 10,000-30,000 |
| Armored boots and gloves | 20,000-35,000 |
| Belt, holster, scabbard | 15,000-30,000 |
| Power sword | 8,000-18,000 |
| Bolt pistol | 6,000-14,000 |
| Rosette and optional relic | 5,000-15,000 |
| Purity seals and parchment | 5,000-12,000 |
| Hair and beard cards | 30,000-60,000 |

Rules:

* Do not waste triangles on hidden surfaces.
* Face, armor silhouette edges, pauldrons, cloak hem, weapons, and rosette get priority.
* Armor bevel detail can be baked where practical.
* Hair and beard cards must be budgeted honestly.
* Chains, if approved, must be optimized and not become a triangle sink.
* Do not chase a low triangle count if it damages portfolio quality.

## LOD Plan

Required for v1:

* LOD0 only

Optional for later:

* LOD1 for portfolio breakdown
* Simplified prop or turntable export

Reason:

The main portfolio goal is a strong hero asset. Full production LOD chains are useful but not mandatory for this stage.

If LOD1 is created later:

* Reduce hair cards first
* Simplify cloak interior and hidden areas
* Reduce armor support loops
* Reduce chain complexity if chains are approved
* Keep face quality acceptable
* Preserve silhouette

## Texture Set Plan

Recommended v1 texture sets:

1. Head and skin
2. Hair and beard
3. Under-armor layer
4. Power armor and metal trim
5. Cloak and hood
6. Optional tabard / chains if approved
7. Leather goods, belt, holster, scabbard
8. Weapons
9. Rosette, optional relic, purity seals, parchment

Recommended resolution:

| Texture Set | Recommended Resolution |
|---|---:|
| Head and skin | 4K |
| Hair and beard | 4K or 2K depending on card density |
| Under-armor layer | 2K-4K |
| Power armor and metal trim | 4K |
| Cloak and hood | 4K |
| Optional tabard / chains | 2K-4K |
| Leather goods / belt / holster / scabbard | 4K |
| Weapons | 2K-4K |
| Rosette / relic / seals / parchment | 2K-4K |

Rules:

* Use 4K for portfolio close-ups where justified.
* Small props may use 2K if they do not require close-up renders.
* Do not give every small object its own 4K texture set.
* Face, power armor, cloak, rosette, and weapons must hold up in close-up.

## UV Strategy

Final game-ready UV rule:

Use 0-1 UV texture sets.

UDIM rule:

UDIMs may be used during high-poly or texturing exploration only if they are later baked or converted into practical game-ready texture sets.

UV priorities:

1. Face
2. Beard and hairline areas
3. Power armor chest
4. Pauldrons
5. Cloak front and silhouette edges
6. Rosette and authority zone
7. Weapons
8. Hands and armored gloves
9. Armored boots
10. Back-of-cloak areas
11. Hidden interior surfaces

UV rules:

* Keep texel density consistent inside each material group.
* Give hero close-up areas higher texel density.
* Keep seams away from focal areas where possible.
* Use straightened UV shells for hard-surface armor where practical.
* Avoid wasting UV space on hidden geometry under armor or cloak.
* Name UV sets and materials clearly.

## Bake Map Requirements

Required bake maps:

* Normal
* Ambient occlusion
* Curvature
* Position
* Material ID

Optional bake maps:

* Thickness
* Height
* Bent normal
* Object-space normal

Normal format:

* DirectX normal format for Marmoset / Unreal workflow unless the final renderer requires otherwise

Bake rules:

* Lock the normal format before baking.
* Do not mix OpenGL and DirectX normal maps inside the same project.
* Test bake one armor piece before baking the full character.
* Test bake one cloth/leather piece before baking the full costume.
* Check hard edges, cage projection, skewing, and seam artifacts.
* Face, power armor chest, shoulder armor, cloak edges, weapons, holster, scabbard, and rosette must be artifact-free.

## Material And Shader Plan

Primary workflow:

* PBR metallic/roughness workflow

Core texture channels:

* Base Color
* Normal
* Roughness
* Metallic
* Ambient Occlusion
* Opacity where needed
* Height only where useful
* Emissive only for optional activated power sword breakdown render

Packed map recommendation:

Use packed ORM where practical:

* R = Ambient Occlusion
* G = Roughness
* B = Metallic

Material families:

* Mature skin
* Hair and beard cards
* Under-armor fabric / flexible material
* Blackened gunmetal power armor
* Tarnished brass / aged gold trim
* Heavy cloak cloth
* Leather
* Parchment
* Deep red wax seals
* Optional chain metal
* Glass or lens material only if justified

Rules:

* Materials must read correctly under neutral lighting before cinematic lighting.
* Do not rely on bloom, smoke, or color grading to hide weak materials.
* Wear must follow physical contact logic.
* Armor should look expensive, ceremonial, battle-used, and maintained.
* Dirt belongs mostly in seams, cloak lower areas, recesses, and contact points.
* No readable text until approved.
* No fake symbols or random inscriptions.

## Skin Technical Target

Skin priority:

Very high.

Reason:

The face is the hero asset.

Requirements:

* Mid-to-late 40s mature skin
* Subtle pores
* Under-eye fatigue
* Realistic color variation
* Controlled roughness variation
* Subtle scars or marks that support veteran character
* Realistic beard transition zones
* No beauty-filtered skin
* No extreme injury or gore

Shader target:

* Marmoset skin shader or equivalent setup
* Subsurface scattering or skin transmission if available and controlled
* Proper roughness breakup
* No waxy plastic skin

## Hair And Beard Technical Target

Recommended v1 method:

Hair cards.

Reason:

Hair cards are game-ready, compatible with Marmoset, and suitable for portfolio breakdowns.

Early test requirement:

Create a rough beard and hair test during the head likeness stage.

Reason:

The beard changes the jawline, mouth read, age read, and Cavill-inspired likeness. Do not wait until the end to test it.

Final groom requirements:

* Short-to-medium dark hair
* Disciplined beard or short facial hair
* Natural breakup
* Slight field imperfection
* Subtle grey allowed if it supports age and authority
* Good hairline transition
* Beard must support the jaw, not hide a weak sculpt

Avoid:

* Overly perfect salon hair
* Barbarian hair
* Giant fantasy beard
* Hair cards that look like flat ribbons
* Groom that hides the face

## Cloth Technical Target

Marvelous Designer status:

Required for the cloak, hood, and possible tabard.

Reason:

The long cloak is one of the most important silhouette assets. Pattern-based construction will produce more believable weight, seams, folds, and cloth logic than manual sculpting alone.

Recommended cloth workflow:

1. Pattern and simulate cloak in Marvelous Designer
2. Include hood resting behind the head or on the upper back
3. Explore tabard only if approved during visual exploration
4. Export high-resolution cloth
5. Clean and refine folds in ZBrush
6. Retopologize for game-ready mesh
7. Preserve important seam and attachment logic
8. Bake cloth detail cleanly

Cloth rules:

* Cloak must feel heavy, ceremonial, and battle-used.
* Hood must rest naturally and must not cover the face in the primary render.
* Folds must follow gravity and material thickness.
* Cloth must not clip through armor, belt, sword, pistol, seals, or boots.
* Final folds should support the standing authority pose.

## Power Armor Technical Target

Armor modeling approach:

* Clean hard-surface modeling
* Human-scale proportions
* Support loops or bevels where needed
* High-poly bevel detail baked to low-poly where practical
* Controlled edge wear
* No Space Marine backpack or power unit silhouette

Armor assets:

* Chest and torso armor
* Pauldrons
* Bracers and armored gloves
* Thigh and knee armor
* Lower-leg armor
* Heavy armored boots
* Compact rear armor structure without Astartes silhouette

Rules:

* Armor must read as custom Inquisitorial power armor.
* Armor must not read as Space Marine armor.
* Pauldrons must be powerful but human-scale.
* Neck, jaw, and face must remain visible.
* No helmet in v1.
* No chapter markings.
* Bevels must bake cleanly.
* Trim must be moderate and purposeful.

## Weapons Technical Target

Approved weapons:

* Main melee: power sword
* Sidearm: bolt pistol

Power sword presentation rule:

* Primary hero render: sword sheathed or held low and inactive
* Secondary close-up render: optional activated blade treatment if approved

Weapon rules:

* Human-usable scale
* Clean silhouette
* Believable grip size
* Believable scabbard / sheath attachment
* Bolt pistol must sit believably in holster
* No oversized fantasy weapon proportions
* No glow effects except optional activated power sword breakdown

Excluded from v1:

* Daemonhammer
* Inferno pistol
* Multiple pistols
* Rifles
* Books as weapon/prop focus

## Rosette, Relic, Seal, And Chain Technical Target

Rosette:

* Mandatory authority object
* Must hold up in close-up
* Should be modeled as a clean hard-surface hero detail
* Placement pending final decision
* Symbol treatment must support safer original version unless fan-art version is clearly separated

Optional relic:

* One maximum
* Pending choice: none, warding reliquary, or sealed document case
* No relic book in v1
* Must fit within scope cap
* Must not require fake readable text
* Must not look Chaos-corrupted or xenos

Purity seals:

* 3 to 5 visible clusters maximum
* Wax and parchment must have proper thickness
* Text remains blank or unreadable until approved
* Placement should support armor, rosette, cloak, or weapon logic

Controlled chain arrangement:

* Pending visual exploration
* Counts as visual design, not automatically a relic
* Must remain secondary to face, power armor, cloak, and rosette
* Must not create Chaos-adjacent, fantasy executioner, or cluttered read

## Rigging And Pose Requirements

Animation requirement:

Not required for v1.

Rigging requirement:

Basic pose rig only.

Recommended method:

* Basic skeleton in Blender or Maya
* Auto-rig acceptable for pose only
* Manual cleanup on shoulders, elbows, wrists, hips, knees, ankles, cloak, and belt if needed
* No full production animation rig required

Minimum requirement:

The model must support a clean standing authority pose without obvious mesh collapse, clipping, or broken weapon contact.

Topology must support:

* Head and neck turn if needed
* Shoulder and elbow pose
* Wrist and hand pose
* Cloak panel deformation or posed sculpt cleanup
* Belt and holster stability
* Scabbard stability
* Weapon grip or near-grip relationship

## Export Requirements

Primary export formats:

* FBX for final mesh export
* OBJ only for high-poly transfers when needed
* PNG or TGA for texture maps
* Marmoset scene file for final presentation

Naming rule:

Use clear asset, stage, and version names.

Example:

```text
black_verdict_character_lowpoly_v001.fbx
black_verdict_head_textures_4k_v001
black_verdict_power_armor_lowpoly_v003.fbx
black_verdict_cloak_lowpoly_v002.fbx
black_verdict_rosette_texture_v002.spp
```

Export rules:

* Freeze or apply transforms before final export.
* Keep scale consistent in centimeters.
* Name meshes clearly.
* Name materials clearly.
* Remove unused hidden geometry.
* Keep high-poly, low-poly, bake, texture, and presentation exports separate.

## File Backup And Version Control

Backup rule:

Working files must be backed up weekly at minimum.

Milestone backup rule:

Back up milestone files immediately and never overwrite them.

Required milestone backups:

* Reference board approved
* Body blockout approved
* Head likeness blockout approved
* Power armor silhouette approved
* Cloak / hood blockout approved
* Authority zone approved
* High-poly approved
* Retopology approved
* UVs approved
* Final bakes approved
* Final textures approved
* Final renders approved

Storage recommendation:

* Local working drive
* External backup
* Cloud backup if available

Do not rely on only one copy of the project.

## Presentation Technical Targets

Primary presentation environment:

Marmoset Toolbag.

Required render set:

* Full-body hero render
* Front view
* Side view
* Back view
* Three-quarter view
* Face close-up
* Power armor close-ups
* Cloak and hood close-up
* Belt, rosette, weapon, scabbard, and holster close-up
* Material close-ups
* Wireframe or topology breakdown
* Texture flats
* Sculpt breakdown

Optional render:

* Activated power sword close-up
* Tabard / chain exploration breakdown if used
* Fan-art vs safer original version comparison if needed

Lighting reference requirement:

Collect 3-5 lighting references before final lookdev.

Recommended lighting directions:

* Cinematic key and rim light
* Neutral studio character lighting
* Dark gallery-style portfolio lighting
* Close-up face lighting
* Material inspection lighting

Presentation budget:

Reserve at least 20-30 hours for final lookdev, lighting, framing, rendering, and breakdown preparation.

Do not rush presentation. Weak final renders can make strong assets look average.

## Technical Risks

### Risk 1: Overbuilding The Asset

Problem:

Too many meshes, props, materials, chains, seals, and texture sets.

Control:

Use the asset checklist and prop cap.

### Risk 2: Space Marine Drift

Problem:

Power armor, shoulders, boots, and rear armor slowly become Astartes-like.

Control:

Keep human proportions visible. Check head size, shoulder width, boot size, and rear silhouette often. Do not add Space Marine backpack or power unit silhouette.

### Risk 3: Chain Overload

Problem:

Controlled chains can become visually impressive but may quickly create clutter, fantasy executioner language, or Chaos-adjacent read.

Control:

Use chains only if they improve silhouette and authority. Keep them secondary to face, power armor, cloak, and rosette.

### Risk 4: Texture Set Inflation

Problem:

Every small object gets its own 4K texture set.

Control:

Group small props logically.

### Risk 5: Hair Cost Underestimated

Problem:

Hair and beard cards take longer than expected and affect likeness.

Control:

Do early groom tests during the head stage.

### Risk 6: Cloak Becomes Too Heavy

Problem:

Cloak mesh becomes dense, hard to retopo, or hard to pose.

Control:

Plan Marvelous Designer output carefully and retopologize cleanly.

### Risk 7: Marmoset And Unreal Split

Problem:

Trying to support both renderers at once creates duplicate work.

Control:

Use Marmoset as v1 target. Treat Unreal as optional later.

### Risk 8: Fake Game-Ready Claim

Problem:

The final result looks good but has bad topology, UVs, bakes, or materials.

Control:

Include topology, UV, texture, and bake breakdowns in the final presentation.

## Remaining Technical Decisions

These must be resolved before final production lock:

1. Pauldron shape
2. Rosette placement
3. Optional relic: none, warding reliquary, or sealed document case
4. Tabard versus controlled chain arrangement
5. Cloak attachment method
6. Exact texture set count after asset checklist
7. Final triangle target after blockout
8. Whether Unreal Engine presentation is added after Marmoset
9. Exact fan-art versus safer original symbol treatment
10. Whether readable inscriptions are used at all
11. Final presentation pose

## Recommended Next File

Update next:

`07_asset_checklist.md`

Reason:

The asset checklist must reflect the approved power armor pivot, cloak, hood, power sword, bolt pistol, scabbard, holster, limited purity seals, and pending tabard/chain exploration before blockout begins.
