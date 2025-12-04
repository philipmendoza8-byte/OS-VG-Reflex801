Master_FieldIndex_v2.1.md

Reflex801 — Master Field Index (HL + LL + Field Study)
Version 2.1 — Standard Custodian Edition
Last Update: 2025-12-04
Operator: philipmendoza8 (Human CoWoS™)
Custodian Engine: Reflex801 Spine v2.1

0. Purpose

Unified master index for all field-lineage materials in Reflex801:
HL (Human Land), LL (Land Lens), RAW → READY lineage, Identity Blocks, and Field Study Modules.

Goal: Any operator must be able to find the correct path in ≤ 60 seconds.
This file is the root navigation spine for humans.

1. Overview

This index anchors the entire reflex field stack:

Human Land (HL)

Land Lens (LL)

Field Study Packages (Demo Modules)

VoiceGold-linked materials (future extension)

Reflex801 = Human CoWoS™ — Human Chip-on-World-on-System.

2. Field Index Structure
ROOT/
│
├── HL/                           # Human Land
│   ├── HL_RAW_IMAGES/
│   ├── HL_Overlay/
│   ├── HL_Annotated/
│   ├── HL_Export/
│   └── HL_Index.md
│
├── LL/                           # Land Lens
│   ├── LL_Map/
│   ├── LL_PointSignals/
│   ├── LL_AreaSignals/
│   ├── LL_Overlay/
│   └── LL_Index.md
│
├── FieldStudyPackage/            # Generic field-study demo module
│   ├── RAW/
│   ├── READY/
│   ├── NOTES/
│   └── INDEX_FieldStudy.md
│
└── Master_FieldIndex_v2.1.md     # You are here

3. Core References
3.1 Identity Blocks

Define terminology, identity, and system spine:

Reflex801_Identity_Block_EN.md

Reflex801_Identity_Block_TH.md

Usage:
Single source of truth for naming modules, writing decks, or defining mission identity.

3.2 Notebook & Library References

Reflex801_Notebooks_v1.0.md — Notebook integration & usage notes

Reflex801_VoiceGold_Library_v1.x.md — High-level VoiceGold structure

Purpose: Explain how RAW → READY → LIBRARY lineage is governed.

4. Field Study Modules
4.1 Current Module (Live)

Field Case 000 — Drone Morning Moment
Baseline case for HL → LL linking using a real field capture.

การศึกษาภาคสนาม/20251204_ช่วงเวลาเข้าโดรน/


Notebook reference:
Section in Reflex801_Notebooks_v1.0.md (“Drone Morning Moment morphological notes”).

4.2 Pattern for All Future Cases
การศึกษาภาคสนาม/
   └── YYYYMMDD_<short_case_code>/
        ├── RAW/          # original captures
        ├── READY/        # cleaned, named, ready for analysis
        ├── NOTES/        # transcripts, sketches
        └── INDEX_<case>.md


All future cases must follow this exact structure for consistency across the system.

5. Usage Notes

Do not rename this file without updating all decks referencing the Master Field Index.

When adding new modules (HL/LL extension or Field Study Case):

Create/update its local INDEX_*.md inside the folder.

Add a short entry under Section 4 here.

This file is the map for humans.
The repo may grow indefinitely, but navigation must remain ≤ 1 minute.

End of Master_FieldIndex_v2.1.md
Reflex801 — Custodian OS™
