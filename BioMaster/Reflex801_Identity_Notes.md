# Reflex801 Identity Notes – v1.0

These notes define how **Reflex801 / VoiceGold** should be understood at a system level.

---

## 1. Core Identity

- **Name:** Reflex801  
- **Layer:** System Spine / Local OS  
- **Domain:** Ground‑truth data from Thai SMEs and everyday life  
- **Mission:** Turn “Human Land” signals into structured assets that AI systems can trust.

Reflex801 is not a SaaS product, an app, or a monolithic platform.  
It is a **way of arranging reality into files, folders, and rules** so that:

1. Every field case can be traced (who / where / when / consent).
2. Every AI output can be cross‑checked against real evidence.
3. Every participant (especially small vendors) can see how their voice is used.

---

## 2. Key Concepts

### Human Land (HL)
- The raw layer: voices, photos, short clips, smells of the market (described in text), informal notes.
- Stored in simple trees: date, location, case code.
- Priority: authenticity over polish.

### Land Lens (LL)
- The interpretive layer: tags, metadata, JSON, Markdown summaries, economic framing.
- LL does *not* overwrite HL – it sits on top as a lens.
- Multiple LLs can exist on one HL set (e.g. economic lens, social lens, product lens).

### VoiceGold
- The subset of HL that comes from **voices** (spoken language, ambient sound with meaning).
- After transcription + minimal cleaning, it becomes tagged LL material.
- VoiceGold is both:
  - A *data type* (voices → text → tags), and
  - A *philosophy* (voice as value, not noise).

### Custodian
- The human (currently: Phillip “Lung” Mendoza) who carries final responsibility for:
  - Consent logic
  - PDPA‑style privacy
  - Transparency to field participants
- In future, this role can be shared / rotated, but must never be absent.

---

## 3. Architectural Principles

1. **Local System First**
   - Assume low‑budget, low‑infrastructure environments.
   - Use tools that can survive bad internet and simple devices.

2. **Traceable by Design**
   - Naming conventions embed time, location, case codes.
   - Every HL asset can be linked back from any LL or deck.

3. **Model‑Agnostic**
   - The system is built to work with *any* AI vendor (OpenAI, Google, Anthropic, DeepSeek, etc.).
   - No exclusive coupling to a single model or platform.

4. **Ethics Before Scale**
   - If a use‑case violates dignity or consent, it is rejected – regardless of ROI.
   - Small, honest datasets are preferred over massive, unclear ones.

---

## 4. Relationship to GENVOZ

- **GENVOZ** = a specialized module that takes VoiceGold streams and transforms them into **economic meaning frames** (e.g. household stress, local optimism, demand signals).
- Reflex801 is the OS; GENVOZ is an **app / analysis stack** running on top of it.
- Output of GENVOZ feeds back into:
  - Local SMEs (practical decisions)
  - Decks for policy / VC / CSR
  - Benchmarks to test how well AI models can align with ground truth

---

## 5. How to Explain Reflex801 in One Minute

> “Reflex801 is a field OS that turns the voices and everyday struggles of Thai SMEs into structured data that AI can trust. Human Land is where we collect the real stories; Land Lens is how we tag and interpret them. VoiceGold is the part that comes from literal voices. Everything is governed by a Custodian so that the people who create the data are never erased from the picture.”

This file should be kept short, updated carefully, and used as the primary identity reference when others ask: **“What is 801, really?”**
