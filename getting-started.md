# 🚀 เริ่มต้นที่นี่ (Start Here)

สวัสดีครับ Sun! นี่คือ package ที่เตรียมไว้สำหรับ deploy นามบัตรออนไลน์ขึ้น GitHub Pages

## 📂 มีอะไรอยู่ในโฟลเดอร์นี้บ้าง

| ไฟล์ | คำอธิบาย |
|---|---|
| `index.html` | ✨ Landing page หลัก — ไฟล์ที่จะแสดงเป็นเว็บไซต์ |
| `business-card.png` | รูปนามบัตรที่จะแสดงในหน้า hero |
| `qr-generator.html` | 🎨 Tool สำหรับสร้าง QR code มีโลโก้ Senestia ตรงกลาง |
| `README.md` | คำอธิบายโปรเจกต์ (จะแสดงบนหน้า GitHub repo) |
| `CLAUDE.md` | 🤖 คำแนะนำสำหรับ Claude Code |
| `DEPLOYMENT.md` | 📖 คู่มือ deploy แบบ step-by-step (ทั้ง manual และ Claude Code) |
| `claude-code-prompt.md` | 📋 Prompt สำเร็จรูปสำหรับ copy ไปวางใน Claude Code |
| `LICENSE` | MIT License |
| `.gitignore` | บอก Git ว่าไฟล์ไหนไม่ต้องเก็บ |
| `getting-started.md` | 👋 ไฟล์ที่คุณกำลังอ่านนี้ |

---

## ⚡ ทำงานเร็วที่สุด (5 ขั้นตอน)

### 1️⃣ ตรวจสอบสิ่งที่ต้องมี

- [ ] **GitHub account** — ถ้ายังไม่มี สมัครที่ https://github.com/join (ฟรี)
- [ ] **Git** — เช็คโดยพิมพ์ `git --version` ใน terminal ถ้าไม่มี ติดตั้งจาก https://git-scm.com
- [ ] **Claude Code** — ติดตั้งแล้วใช่ไหม? ถ้ายัง: `npm install -g @anthropic-ai/claude-code`

### 2️⃣ ดาวน์โหลดโฟลเดอร์นี้ลงเครื่อง

เก็บไว้ที่ไหนก็ได้ที่หาเจอง่าย ๆ เช่น:
- `~/Documents/digital-card/`
- `~/Projects/noppon-card/`

### 3️⃣ เปิด Claude Code ในโฟลเดอร์นี้

```bash
cd path/to/digital-card
claude
```

### 4️⃣ Copy prompt ไปวาง

เปิดไฟล์ `claude-code-prompt.md` → copy **Prompt 1: Full Deployment** → แทน `[YOUR_GITHUB_USERNAME]` ด้วย username จริงของคุณ → paste ใน Claude Code

### 5️⃣ ทำตามที่ Claude Code บอก

Claude จะถามและทำให้คุณทุกอย่าง ใช้เวลาประมาณ 10-15 นาที

---

## 📋 ตัวอย่าง Username ที่แนะนำ

ถ้ายังไม่มี GitHub username แนะนำตั้งชื่อแบบ professional:

- ✅ `nopponsiangchin` — ใช้ชื่อจริงเต็ม
- ✅ `noppon-s` — ย่อนามสกุล
- ✅ `sun-siangchin` — ใช้ชื่อเล่น + นามสกุล
- ❌ `sun_hacker_2025` — ดูไม่ professional
- ❌ `xXSunXx` — ไม่เหมาะกับงาน

---

## 🎯 ผลลัพธ์ที่คุณจะได้

หลัง deploy เสร็จ คุณจะได้:

1. **URL สำหรับ landing page** เช่น `https://nopponsiangchin.github.io/noppon-siangchin/`
2. **QR code พร้อมโลโก้ Senestia** ตรงกลาง — สร้างจาก `qr-generator.html`
3. **Wallpaper สำหรับมือถือ/laptop** — มี QR code ฝังอยู่ ขนาด 2880×1800
4. **vCard download function** — ลูกค้ากดปุ่ม Save Contact แล้วเซฟเข้ามือถือได้ทันที

---

## 🆘 ถ้าติดปัญหา

**ปัญหาที่พบบ่อย:**

| ปัญหา | วิธีแก้ |
|---|---|
| `git: command not found` | ติดตั้ง Git จาก https://git-scm.com |
| `claude: command not found` | `npm install -g @anthropic-ai/claude-code` |
| Permission denied ตอน push | ใช้ Personal Access Token แทน password — สร้างที่ https://github.com/settings/tokens |
| Site ไม่แสดงหลัง enable Pages | รอ 2-5 นาที แล้ว refresh |
| ภาพไม่ขึ้น | ตรวจชื่อไฟล์ (case-sensitive) `business-card.png` ไม่ใช่ `Business-Card.PNG` |

ถ้ายังแก้ไม่ได้ ใช้ **Prompt 4: Troubleshooting** ใน `claude-code-prompt.md`

---

## 🎁 Bonus: หลัง deploy เสร็จ

1. **ทดสอบ URL บนมือถือจริง** — เปิดทั้ง iPhone และ Android เช็คว่าโหลดได้
2. **เปิด `qr-generator.html`** → ใส่ URL ใหม่ → ดาวน์โหลด QR PNG
3. **อัปเดต LinkedIn** — ใส่ URL ใน Contact Info section
4. **บันทึก URL ไว้ใน Notion** เพื่อใช้อ้างอิงในอนาคต
5. **(Optional)** ซื้อ custom domain เช่น `noppon.dev` แล้วผูกกับ repo นี้

---

ขอให้ deploy สำเร็จครับ! 🎉

Sun
