# GENVOZ SystemCheck v1.0  
(Engine Mount + Wiring Harness – Stability Mode)

> ไฟล์นี้มีหน้าที่เหมือน “ช่างเช็กเครื่อง” หลังติดตั้ง GENVOZ core v1.0 แล้ว  
> ใช้ยืนยันว่าทั้งโครง + สายไฟ + เอกสารทุกชิ้น อยู่ครบและทำงานใน ecosystem Reflex801 ได้จริง

---

## 0. Metadata

- **โมดูล:** GENVOZ v1.0  
- **โฟลเดอร์หลัก:** `GENVOZ/`  
- **ไฟล์ชุด core:** 8 ไฟล์ (Concept → SampleCase)  
- **สถานะชุดนี้:** ✅ ติดตั้งแล้วที่สาขา `main`  
- **ไฟล์ระบบนี้:** `GENVOZ_SystemCheck_v1.0.md`  
- **วันที่ออกแบบชุดตรวจ:** 2025-12-09  

---

## 1. Installation Snapshot (File Presence Check)

เช็กลิสต์ด้านล่าง = ตรวจว่า “เครื่องในห้องเครื่อง” อยู่ครบทุกชิ้น

| # | Expected file name | Path ใน repo | Status |
|---|--------------------|-------------|--------|
| 1 | `GENVOZ_Concept_Overview_TH_EN.md` | `GENVOZ/` | ⬜ |
| 2 | `GENVOZ_FieldCase_Template.md` | `GENVOZ/` | ⬜ |
| 3 | `GENVOZ_LayerSchema_v1.0.md` | `GENVOZ/` | ⬜ |
| 4 | `GENVOZ_MasterIndex.md` | `GENVOZ/` | ⬜ |
| 5 | `GENVOZ_MasterPrompt_v1.0.md` | `GENVOZ/` | ⬜ |
| 6 | `GENVOZ_NotebookLM_SystemJSON.json` | `GENVOZ/` | ⬜ |
| 7 | `GENVOZ_QA_Bridge_TH.md` | `GENVOZ/` | ⬜ |
| 8 | `GENVOZ_SampleCase_ThaiRamanStreet.md` | `GENVOZ/` | ⬜ |

**วิธีใช้:**  
- ทุกครั้งที่ clone / pull repo นี้ไปสาขาใหม่ ให้เปิดไฟล์นี้ แล้วติ๊ก `⬜ → ✅` ด้วยมือตัวเอง  
- ถ้ามีไฟล์ไหนหาย ให้ **หยุด** ใช้งาน GENVOZ บนสาขานั้นก่อน แล้ว sync จากแหล่งที่ถือว่าเป็น “เครื่องแม่”

---

## 2. Wiring Harness Check (Logical Consistency)

เช็คว่า “สายไฟเชื่อมถึงกัน” ระหว่างแต่ละไฟล์

1. **MasterIndex → ไฟล์อื่น**
   - เปิด `GENVOZ_MasterIndex.md`  
   - ตรวจว่าใน MasterIndex มีการอ้างถึงทั้ง 7 ไฟล์อื่นของ GENVOZ ครบ (Concept, Template, Schema, Prompt, JSON, QA, SampleCase)  
   - ถ้าขาดไฟล์ไหน ให้กลับมาแก้ MasterIndex ให้สอดคล้องกับโครงจริงทันที

2. **LayerSchema ↔ Concept / Prompt**
   - เปิด `GENVOZ_LayerSchema_v1.0.md`  
   - ตรวจชื่อเลเยอร์กับคำอธิบายใน `GENVOZ_Concept_Overview_TH_EN.md` และ `GENVOZ_MasterPrompt_v1.0.md`  
   - ชื่อเลเยอร์ / ภารกิจแต่ละเลเยอร์ควรสะท้อนกัน (คนอ่านไม่งงว่าชั้นไหนทำอะไร)

3. **NotebookLM JSON ↔ เอกสาร**
   - เปิด `GENVOZ_NotebookLM_SystemJSON.json`  
   - ตรวจว่าใน JSON อ้างอิงไฟล์ชุด GENVOZ ถูกต้อง (ถ้ามี path หรือชื่อไฟล์)  
   - ถ้าโยงผิด ให้ถือว่า “สายสัญญาณขาด” ต้องแก้ JSON ก่อนใช้งานจริง

---

## 3. Human-Level Sanity Test (Quick NLM Check)

ทดสอบแบบ “ควันแรกจากท่อไอเสีย” ว่าโมดูลตอบสนองได้ตามที่ตั้งใจ

ให้เลือก NLM ใดก็ได้ที่ลุงใช้เป็นหลัก แล้วรัน 3 เทสนี้:

### Test A — Concept Integrity

**Prompt ตัวอย่าง**  

> “อ่านไฟล์ `GENVOZ/GENVOZ_Concept_Overview_TH_EN.md` แล้วสรุปให้ 5 bullet (TH) ว่า  
> GENVOZ คืออะไร และทำหน้าที่อะไรในระบบ Reflex801 / VoiceGold”

**ผ่านเมื่อ**  
- AI อธิบายว่า GENVOZ คือ *Economic Voice Analysis Layer* หรือความหมายใกล้เคียง  
- มีการพูดถึงว่า GENVOZ ทำงาน “บน” Reflex801 / VoiceGold (ไม่ใช่ของคนละจักรวาล)

---

### Test B — Layer & Prompt Cohesion

**Prompt ตัวอย่าง**  

> “อ่านไฟล์ `GENVOZ/GENVOZ_LayerSchema_v1.0.md` และ  
> `GENVOZ/GENVOZ_MasterPrompt_v1.0.md` แล้วอธิบาย flow การวิเคราะห์เสียงเศรษฐกิจ  
> เป็น 4–6 ขั้นตอน (TH)”

**ผ่านเมื่อ**  
- คำตอบมีการไล่ลำดับ step ตั้งแต่รับเสียง → ตัดเฟรม → ตีความ → สร้างเลเยอร์ meaning  
- ไม่มีอาการตอบกว้างเกินไปแบบ generic NLP ทั่วไป (ต้องมีคำศัพท์/โครง GENVOZ ปรากฏ)

---

### Test C — SampleCase Consistency (Thai Raman Street)

**Prompt ตัวอย่าง**  

> “อ่านไฟล์ `GENVOZ/GENVOZ_SampleCase_ThaiRamanStreet.md` แล้ว  
> สรุป insight เศรษฐกิจฐานราก 3–5 ข้อ ที่ GENVOZ น่าจะดึงออกมาจากเคสนี้”

**ผ่านเมื่อ**  
- Insight ที่ได้ผูกกับ *พฤติกรรมซื้อจริง* / *สภาพรายได้* / *ความเสี่ยง* ของร้าน/คนในเคส  
- ไม่ใช่แค่สรุปเนื้อเรื่อง แต่สะท้อนโทนเศรษฐกิจแบบที่ Reflex801 สนใจ

---

## 4. Version / Branch Policy (Minimal)

เพื่อไม่ให้ GENVOZ กลายเป็น “ของเละใน trunk”:

1. **สาขาหลัก:**  
   - `main` = รับเฉพาะ GENVOZ เวอร์ชันที่ผ่าน SystemCheck ชุดนี้แล้วเท่านั้น

2. **งานทดลอง / แก้ prompt / แก้ schema:**  
   - ให้แตก branch เช่น `feature/genvoz-prompt-tuning` หรือ `exp/genvoz-layer-v1-1`  
   - เมื่อพร้อมค่อยเปิด PR และแนบผล Test A–C สั้น ๆ ใน description

3. **การเพิ่มไฟล์ใหม่ในโฟลเดอร์ GENVOZ/**  
   - ทุกครั้งต้องอัปเดต `GENVOZ_MasterIndex.md` + เช็กผลกระทบกับ JSON (ถ้ามี)  
   - จากนั้นเพิ่ม checklist ใหม่ในไฟล์ SystemCheck ฉบับถัดไป เช่น `v1.1`

---

## 5. Field Notes (สำหรับเจ้าของระบบ)

ช่องนี้เผื่อให้ลุงเขียนบันทึกสั้น ๆ เวลาเอา GENVOZ ไปติดตั้งในสภาพแวดล้อมใหม่  
(ระบุวันที่ / เครื่องไหน / บริบทไหน / note ความเสถียร)

```text
[ตัวอย่างบันทึก]

2025-12-09 – ติดตั้ง GENVOZ v1.0 บน OS-VG-Reflex801 (main) – ใช้ผ่าน GitHub + NLM Stack เดิม
- ผล Test A–C: ผ่านทั้งหมด / latency ปกติ / ไม่มี error ด้าน path เอกสาร
- Observation: QA_Bridge_TH ใช้อธิบาย GENVOZ ได้เคลียร์มาก → ใช้เป็น anchor prompt ได้ดี
