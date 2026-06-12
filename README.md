# Ceremonial Tea Name Generator 🍵

เครื่องสุ่มชื่อชาเขียวเกรดพิธีการแบบเท่ๆ เบียวๆ — ชื่ออังกฤษ + ชื่อไทยใน 「 」 + เกรดพิธีการ

## Deploy ไป Vercel

ไฟล์เดียวจบ ไม่ต้อง build อะไร เลือกวิธีไหนก็ได้:

**วิธีที่ 1 — Vercel CLI**
```bash
npm i -g vercel
cd ceremonial-tea
vercel
```

**วิธีที่ 2 — Drag & drop**
ลากโฟลเดอร์ทั้งอันไปวางที่ https://vercel.com/new

**วิธีที่ 3 — Git**
push โฟลเดอร์นี้ขึ้น GitHub แล้ว import เข้า Vercel — ตั้ง framework เป็น "Other" (static), ไม่ต้องมี build command

## ปรับแต่ง

คลังคำทั้งหมดอยู่ใน `<script>` ของ `index.html`:
- `prefixEn` / `coreEn` / `midOptions` — ชื่ออังกฤษ
- `prefixTh` / `coreTh` / `placeTh` — ชื่อไทย
- `chaosTh` — วลีต่อท้ายโหมดเบียวสุด
- `ranks` — เกรดพิธีการ
