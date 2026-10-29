# Typing Speed Test — วัดความเร็วพิมพ์ ไทย / อังกฤษ

แบบทดสอบวัดความเร็วการพิมพ์ 2 ภาษา (ไทย + อังกฤษ) รันในเบราว์เซอร์ล้วน ๆ — ไฟล์ HTML เดียว ไม่มี build step ไม่มี dependency

A bilingual (Thai/English) typing speed test that runs entirely in the browser — one self-contained HTML file, zero dependencies.

**Live demo:** https://typing-speed-test-fieldmtws-projects.vercel.app/

## ฟีเจอร์ / Features

- 🇹🇭🇬🇧 ข้อความทดสอบไทย + อังกฤษ (ภาษาละ 6 ข้อความ มีแนวโค้ดด้วย)
- ⏱️ เลือกเวลาได้: 15 / 30 / 60 / 120 วินาที
- 📊 ผลลัพธ์: WPM + ความแม่นยำ + ความสม่ำเสมอ + ตารางผลรอบก่อนหน้าในเซสชัน
- ⌨️ ไฮไลต์ถูก/ผิดแบบเรียลไทม์ทีละตัวอักษร
- 📱 รองรับมือถือ + โหมดมืด

## คิดคะแนนยังไง / How scoring works

- **WPM** = (ตัวอักษรที่ถูก ÷ 5) ÷ นาที — สูตรมาตรฐานสากล
- **ภาษาไทย** นับเป็น "อักขระ" (พยัญชนะ + สระ/วรรณยุกต์ที่ติดกันนับเป็น 1) ด้วย `Intl.Segmenter` แล้วใช้สูตรเดียวกัน — คนทั่วไปพิมพ์ไทยราว 25–35 WPM ส่วนอังกฤษราว 40 WPM
- **ความสม่ำเสมอ (Consistency)** วัดจากความแกว่งของความเร็วในแต่ละช่วงของรอบ — ใกล้ 100% แปลว่านิ้วเดินจังหวะนิ่ง

## วิธีใช้ / Usage

เปิด `index.html` ในเบราว์เซอร์ได้เลย ไม่ต้องรันเซิร์ฟเวอร์
Just open `index.html` in a browser. No server needed.

## เทคโนโลยี / Tech

`index.html` ไฟล์เดียว (HTML + CSS + vanilla JS) — ไม่มี dependency
Single self-contained `index.html` — no dependencies.
