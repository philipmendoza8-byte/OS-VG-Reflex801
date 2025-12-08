# GENVOZ Identity & Link to Reflex801

## 1. What is GENVOZ?

**GENVOZ** is the **Economic Voice Analysis Layer** running on top of Reflex801 / VoiceGold.

Its job is simple to state and hard to do:

> Take messy, real‑world voices from Human Land (HL) and turn them into structured, comparable economic meaning frames.

In practice, GENVOZ:
- Ingests voice logs from small vendors, SMEs, and local actors.
- Uses transcription + tagging prompts (the GENVOZ Master Prompt) to segment and interpret those voices.
- Outputs **4 key layers** (as defined in the GENVOZ design docs):
  1. Time‑segmented meaning units
  2. Emotional / stress signals
  3. Economic context (costs, revenue, risk, opportunity)
  4. Forward‑looking hints (what might change in 1–3 months)

GENVOZ does **not** replace economists or policymakers.  
It gives them a *micro‑signal radar* sourced directly from the field.

---

## 2. Relationship to Reflex801 / VoiceGold

- Reflex801 defines **where and how** data lives (folders, naming, consent, traceability).
- VoiceGold defines **what kind of data** we are focusing on (voices, conversations, ambient sound with meaning).
- GENVOZ defines **how we read those voices economically**.

Diagram in words:

- HL_RAW_VOICE → (stored under Reflex801 naming rules)  
- → VoiceGold (transcribed, lightly cleaned, tagged)  
- → GENVOZ (segmented + interpreted into economic signal layers)  
- → Decks / Dashboards / Alerts (for SMEs, partners, researchers, VCs)

GENVOZ is therefore *not* a separate project; it is a **module** that proves why Reflex801 and VoiceGold matter.

---

## 3. How to Explain GENVOZ in One Sentence

> “GENVOZ listens to the real voices of small businesses and turns them into early‑warning economic signals, running on top of the Reflex801 / VoiceGold field OS.”

Use this file as the identity bridge whenever GENVOZ is mentioned in isolation (e.g. in a deck, forum, or research context). It should always point back to Reflex801 / VoiceGold as the underlying spine.
