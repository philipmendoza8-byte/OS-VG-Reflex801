# GENVOZ Layer Schema v1.0

This file defines the **semantic contract** for GENVOZ outputs.

---

## Overview

GENVOZ organizes each voice-derived case into **segments**, and each segment into **4 layers**:

1. L1 – Narrative Slice
2. L2 – Emotion & Stress
3. L3 – Economic Context
4. L4 – Forward Signal (1–3 months)

The goal is to make outputs:
- Comparable across time, cases, and regions
- Usable by humans (analysts, SMEs, policymakers)
- Machine-readable for dashboards and further modeling

---

## L1 – Narrative Slice

**Purpose:** Capture “what is happening” in plain terms.

Fields (suggested):
- `who` – role of the speaker (e.g., street vendor, farmer, driver, shop owner)
- `topic` – short label for the main subject (e.g., rent pressure, demand drop)
- `what_happened` – 1–3 sentences describing the situation

Constraints:
- No forecasting here.
- Stay as close as possible to the original words.

---

## L2 – Emotion & Stress

**Purpose:** Capture emotional tone and stress level without pathologizing the speaker.

Fields:
- `tone` – free text, short (e.g., “tired but hopeful”, “angry and resigned”)
- `stress_level` – enum: `low | medium | high | unclear`
- `emotion_keywords` – array of 2–6 simple emotion tags
- `notes` – optional clarifications

Constraints:
- Avoid clinical language.
- When uncertain, mark `stress_level: "unclear"` and explain why.

---

## L3 – Economic Context

**Purpose:** Make economic structure visible from the story.

Fields:
- `income_streams` – list of how money comes in (e.g., daily sales, side jobs)
- `cost_drivers` – list of key costs (e.g., rent, fuel, ingredients, school fees)
- `constraints` – structural limits (e.g., debt, illness, location, caregiving)
- `opportunities` – realistic openings mentioned or implied
- `summary` – 2–4 sentences tying the above together

Constraints:
- Focus on what is mentioned or strongly implied by the speaker.
- Do not invent entire business models.

---

## L4 – Forward Signal

**Purpose:** Offer a cautious short-term outlook and identify pivot points.

Fields:
- `short_term_outlook` – enum: `improving | declining | stable | unclear`
- `time_horizon_months` – string, usually `"1-3"`
- `risk_factors` – list of main risks if nothing changes
- `leverage_points` – list of small, concrete changes that might help
- `commentary` – brief explanation tying L1–L3 into the outlook

Constraints:
- Always label this layer as **analysis / inference**, not fact.
- No grand predictions; stay inside the 1–3 month window.

---

## Aggregation Across Segments

For each case, segments can later be aggregated into:
- Case-level stress profile
- Case-level economic pressure map
- Case-level forward risk / opportunity index

That aggregation is **outside** the scope of GENVOZ v1.0 and can be handled by downstream tools.
