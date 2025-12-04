Master_FieldIndex.md

Reflex801 – Master Field Index (HL + LL + Field Study)
Version 2.0 — Clean English Edition

0. Purpose

Unified entry point for all field materials in Reflex801:
HL (Human Land), LL (Land Lens), RAW → READY lineage, Identity Blocks, and Field Study Modules.

This file is the root map for humans.
Goal: Any operator must be able to find the correct path in ≤ 60 seconds.

1. Overview

This index acts as the primary field index for Reflex801.

It anchors:

Human Land (HL)

Land Lens (LL)

Field Study Packages (Demo Modules)

VoiceGold-linked materials (future extension)

Reflex801 = Human CoWoS™ — Human Chip-on-World-on-System.

2. Field Index Structure
ROOT/
│
├── HL/                                # Human Land
│   ├── HL_RAW_IMAGES/
│   ├── HL_Overlay/
│   ├── HL_Annotated/
│   ├── HL_Export/
│   └── HL_Index.md
│
├── LL/                                # Land Lens
│   ├── LL_Map/
│   ├── LL_PointSignals/
│   ├── LL_AreaSignals/
│   ├── LL_Overlay/
│   └── LL_Index.md
│
├── FieldStudyPackage/                 # Generic field-study demo module
│   ├── RAW/
│   ├── READY/
│   ├── NOTES/
│   └── INDEX_FieldStudy.md
│
└── Master_FieldIndex.md               # You are here

3. Core References
3.1 Identity Blocks

These define terminology, identity, and system spine:

Reflex801_Identity_Block_EN.md

Reflex801_Identity_Block_TH.md

Usage:
Single source of truth when naming modules, writing decks, or defining mission identity.

3.2 Notebooks & Library References

Reflex801_Notebooks_v1.0.md — Notebook integration & usage notes

Reflex801_VoiceGold_Library_v1.x.md — VoiceGold library high-level structure (future-ready)

Purpose: Explain how RAW → READY → LIBRARY lineage is tracked.

4. Field Study Modules
4.1 Current Module (Live)

Field Case 000 — Drone Morning Moment
Baseline test case for linking HL → LL using a real field moment.

Main folder:
การศึกษาภาคสนาม/20251204_ช่วงเวลาเข้าโคมด

Notebook link:
Section in Reflex801_Notebooks_v1.0.md (“Drone Morning Moment morphological notes”)

4.2 Pattern for All Future Cases
การศึกษาภาคสนาม/
└── YYYYMMDD_<short_case_code>/
    ├── RAW/       # original captures
    ├── READY/     # cleaned, named, ready for analysis
    ├── NOTES/     # transcripts, quick sketches
    └── INDEX_<case>.md


All future cases must follow this pattern for system consistency.

5. Usage Notes

Do not rename this file without updating all decks that reference the “Master Field Index”.

When a new module (HL/LL extension or Field Study Case) is added:

Create/update its local INDEX_*.md inside its folder.

Add a short entry under Section 4 in this file.

This file is the map for humans.
The repo may grow indefinitely, but navigation must stay ≤ 1 minute.

End of Master_FieldIndex.md (Clean English Version 2.0)
Reflex801 – Custodian OS™
