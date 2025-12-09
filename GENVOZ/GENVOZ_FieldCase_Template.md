# GENVOZ Field Case Template

Use this template whenever you want to run GENVOZ on a new field recording.

---

## 1. Case Metadata

- **Case ID:** `CASE_YYYYMMDD_LOCATION_CODE`
- **Location:** (e.g., Thai Raman Street, Bangkok)
- **Country / Region:** (e.g., Thailand – Bangkok)
- **Speaker Role:** (e.g., noodle vendor, fruit seller, tuk-tuk driver)
- **Recording DateTime (local):** `YYYY-MM-DDTHH:MM:SS+TZ`
- **Recording Length (approx):** (e.g., 07:32 minutes)
- **Language / Dialect:** (e.g., TH – Central, TH – Isan)
- **Consent Note:** brief text confirming informed consent in HL layer.

---

## 2. HL / Raw Voice Summary

- **Context:** (where, when, what was happening around)
- **Key Topics Mentioned:** bullet list
- **Rough Mood:** (your human impression before GENVOZ)

---

## 3. Transcript Source

- **Transcript File:** link / path (e.g., `HL/VOICE/2025/...`)
- **Transcription Method:** (Notta, manual, other)
- **Cleaning Level:** raw | lightly cleaned | heavily edited (aim: raw or light)

Paste transcript (or a relevant excerpt) below if needed:

```text
<raw transcript here>
```

---

## 4. GENVOZ Config for This Run

- **Model:** (e.g., GPT, Claude, Gemini, DeepSeek – any)
- **Prompt Version:** `GENVOZ_MasterPrompt_v1.0`
- **Language of Output:** same as transcript / bilingual / EN only
- **Max Segments (soft target):** (e.g., 10–20)

---

## 5. GENVOZ Output (JSON)

Paste the JSON output from the model here:

```json
{
  "...": "..."
}
```

---

## 6. Analyst Notes (Optional)

- What surprised you?
- Did GENVOZ miss anything important from the human point of view?
- What follow-up questions would you ask the speaker next time?
