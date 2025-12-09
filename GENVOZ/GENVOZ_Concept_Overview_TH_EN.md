# GENVOZ Concept Overview – TH / EN

---

## TH – GENVOZ คืออะไร

**GENVOZ** คือ “ชั้นวิเคราะห์เสียงเศรษฐกิจ” ที่วิ่งอยู่บนสันหลังระบบ **Reflex801 / VoiceGold**  
หน้าที่ของ GENVOZ คือ:

> แปลงเสียงจริงจากสนาม (แม่ค้า, SME, คนทำมาหากิน) ให้กลายเป็น “เฟรมความหมายทางเศรษฐกิจ” ที่เปรียบเทียบข้ามเวลาและข้ามพื้นที่ได้

GENVOZ ไม่ใช่โมเดล AI แยกต่างหาก แต่เป็น **ชุดกติกา + โครงสร้างผลลัพธ์** ที่สั่งให้ AI ทุกค่าย:

1. ฟังเสียง → แบ่งช่วงตามความหมาย (เช่น 4 / 8 / 10 วินาทีต่อเฟรม)
2. สกัดความหมายสำคัญในแต่ละช่วง
3. แปลงเป็น 4 ชั้นหลัก (Layer 1–4)

### 4 Layers ของ GENVOZ (เวอร์ชันย่อ)

1. **L1 – Narrative Slice (เศษเรื่องเล่า)**
   - ใครพูด, พูดถึงอะไร, เกิดอะไรขึ้นในช็อตสั้น ๆ
2. **L2 – Emotion & Stress (อารมณ์ / ความตึงเครียด)**  
   - โทนเสียง, ความกังวล, ความหวัง, การยอมแพ้ / ฮึดสู้
3. **L3 – Economic Context (บริบททางเศรษฐกิจ)**  
   - ต้นทุน, รายได้, ความเสี่ยง, ปัจจัยที่กดดัน เช่น หนี้, ดอกเบี้ย, ค่าเช่า
4. **L4 – Forward Signal (สัญญาณล่วงหน้า)**  
   - ถ้าไม่มีอะไรเปลี่ยน → อีก 1–3 เดือนชีวิตเขาจะดีขึ้น แย่ลง หรือคงที่
   - อะไรคือ “จุดเปลี่ยน” ที่จะทำให้กราฟชีวิตเขาเบนทาง

GENVOZ จึงเป็นเหมือน “เครื่องมืออ่านเสียง” ที่ทำงานตามกติกา 801  
ไม่แย่งงานนักเศรษฐศาสตร์ แต่ช่วยเพิ่ม “สัญญาณระดับดิน” ให้คนที่ตัดสินใจบนโต๊ะ

---

## EN – What is GENVOZ?

**GENVOZ** is the **Economic Voice Analysis Layer** that runs on top of **Reflex801 / VoiceGold**.  
Its core mission is:

> To turn real-world voices from the field (vendors, SMEs, everyday workers) into structured economic meaning frames that are comparable across time and space.

GENVOZ is not a standalone AI model. It is a **set of rules + output schema** that instructs any LLM to:

1. Listen to voice-derived text → segment it into meaning units (4 / 8 / 10 seconds each).
2. Extract key meaning per segment.
3. Map each segment into **four layers (L1–L4)**:

   1. **L1 – Narrative Slice**  
      - Who is speaking, about what, what is happening in this brief slice.
   2. **L2 – Emotion & Stress**  
      - Tone, worry, hope, resignation, determination.
   3. **L3 – Economic Context**  
      - Costs, revenue, risk factors, debt pressure, rent, interest, etc.
   4. **L4 – Forward Signal**  
      - Given the current trajectory, what is likely in 1–3 months?  
        What are the “pivot points” that could change the curve?

GENVOZ does not replace economists. It provides a **micro-signal radar** from “Human Land” so that economic analysis, policy, and investment decisions can be anchored in lived experience.

This file should be used whenever someone asks for a **high-level explanation** of GENVOZ.
