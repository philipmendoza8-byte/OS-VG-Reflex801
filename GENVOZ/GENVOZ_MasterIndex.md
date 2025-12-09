# GENVOZ Master – Index

This folder is the **master entry point** for everything related to **GENVOZ** –  
the Economic Voice Analysis Layer running on top of Reflex801 / VoiceGold.

All files here are:
- Plain text (`.md` / `.json`, UTF-8)
- Git-ready
- Safe to feed into AI tools (NotebookLM, GPT, etc.) as **system context**

---

## File Map

1. **GENVOZ_Concept_Overview_TH_EN.md**
   - Short concept explainer in both TH + EN
   - Use when someone asks: “GENVOZ คืออะไร / What is GENVOZ?”

2. **GENVOZ_MasterPrompt_v1.0.md**
   - The core multi-part prompt for GENVOZ
   - Defines segmentation, 4-layer meaning structure, and output style
   - Designed to be copy–paste friendly into any LLM

3. **GENVOZ_LayerSchema_v1.0.md**
   - Human-readable schema for GENVOZ outputs
   - Defines each layer (L1–L4), fields, and example values

4. **GENVOZ_FieldCase_Template.md**
   - Template for running a GENVOZ pass on a single field case (หนึ่งเคส)
   - Includes: metadata, raw voice description, model config, outputs, notes

5. **GENVOZ_NotebookLM_SystemJSON.json**
   - System-to-system `.json` describing GENVOZ for tools like NotebookLM
   - Contains: name, version, layers, field schemas, and example queries

6. **GENVOZ_SampleCase_ThaiRamanStreet.md**
   - Sample (dummy) case structure based on “Thai Raman Street” type scenario
   - Shows how GENVOZ attaches to a real HL case in Reflex801 style

7. **GENVOZ_QA_Bridge_TH.md**
   - Notes about **คำถาม–คำตอบ (Q&A)** pattern in Thai
   - Common pitfalls and how GENVOZ should handle “ถาม–ตอบแบบไทย ๆ”

---

## Usage

- For **first-time readers** → start with:
  - `GENVOZ_Concept_Overview_TH_EN.md`
  - `GENVOZ_LayerSchema_v1.0.md`
- For **LLM configuration** → use:
  - `GENVOZ_MasterPrompt_v1.0.md`
  - `GENVOZ_NotebookLM_SystemJSON.json`
- For **field work / examples** → use:
  - `GENVOZ_FieldCase_Template.md`
  - `GENVOZ_SampleCase_ThaiRamanStreet.md`

---

Last updated: 2025-12-08
System: Reflex801 / VoiceGold – GENVOZ Master
Custodian: Phillip “Lung” Mendoza
