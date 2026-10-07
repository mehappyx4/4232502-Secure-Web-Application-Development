# 🎓 Student Portfolio & Digital Skill Passport

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)

ระบบ **Student Portfolio & Digital Skill Passport** - เว็บแอปพลิเคชันพอร์ตโฟลิโอนักศึกษาดิจิทัลรูปแบบใหม่ รวมระบบยืนยันตัวตนดิจิทัล สถิติทักษะ โปรเจกต์ เกียรติบัตร เหรียญรางวัล (Badges) และเครื่องมือสร้าง Resume ในตัว

---

## 🌟 ฟีเจอร์หลัก (Key Features)

### 🪪 1. Digital Student Passport & SSO
- **บัตรประจำตัวนักศึกษาดิจิทัล**: แสดงข้อมูลส่วนตัว รหัสนักศึกษา คณะ/สาขา เกรดเฉลี่ย (GPAX) และระดับ Skill Level
- **SHA-256 Verification**: ลายเซ็นอิเล็กทรอนิกส์ยืนยันความถูกต้องของข้อมูล พร้อมฟังก์ชันคัดลอก Hash
- **University SSO Simulation**: ระบบจำลองการเข้าสู่ระบบด้วยบัญชีมหาวิทยาลัย

### 🎯 2. Skill Analytics & Radar Chart
- **การวิเคราะห์ทักษะแบบภาพรวม**: แสดงกราฟ Radar Chart ด้วย Chart.js แบ่งหมวดหมู่ทักษะ (Frontend, Backend, AI/ML, DevOps, Database, Security, UI/UX)
- **Skill Progress Bar**: แถบวัดระดับทักษะพร้อมสถานะการทดสอบ/ยืนยัน

### 💻 3. Projects & GitHub Integration
- **คลังผลงาน (Projects Showcase)**: ค้นหาและกรองผลงานตามหมวดหมู่ (All, Web, Mobile, AI/ML, IoT/Hardware)
- **GitHub Stats & Activity**: จำลองสถิติกิจกรรมบน GitHub (Contributions Graph, Repositories count, Commits)

### 📜 4. Certificates & Digital Credentials
- **ระบบจัดเก็บเกียรติบัตร**: แสดงใบประกาศนียบัตรดิจิทัลพร้อมการยืนยันผู้จัดการทดสอบ (Verified Issuers)
- **Modal Preview**: ดูรูปภาพเกียรติบัตรฉบับเต็มและดาวน์โหลดไฟล์

### 🏆 5. Badges & Gamification
- **เหรียญรางวัลความสำเร็จ**: ระบบปลดล็อก Badge ตาม XP และภารกิจ (เช่น Code Ninja, AI Pioneer, Hackathon Winner)

### 📄 6. Interactive Resume Builder
- **เครื่องมือสร้างและดาวน์โหลด Resume**: เลือกเทมเพลต และส่งออกไฟล์ Resume ได้สะดวก

### 🔐 7. Security & Privacy
- **ความปลอดภัยและการตั้งค่าความเป็นส่วนตัว**: การจัดการสิทธิ์การมองเห็นข้อมูล และ บันทึกกิจกรรมระบบ (Audit Logs)

### 🐍 8. Image Utilities (Python Scripts)
- **Script ลบพื้นหลังรูปภาพอัตโนมัติ** (`scripts/remove_background_auto.py` & `scripts/remove_background_final.py`): ใช้ Python Script ร่วมกับไลบรารี Rembg / PIL สำหรับประมวลผลรูปโปรไฟล์นักศึกษา

---

## 📁 โครงสร้างโปรเจกต์ (Project Structure)

```text
portfolio/
├── index.html                    # หน้าหลัก HTML (รวม Navbar, Tabs, Modals)
├── style.css                     # ไฟล์ตกแต่ง CSS (รองรับ Responsive, Dark UI, Glassmorphic Design)
├── script.js                     # สคริปต์ควบคุมการทำงาน (Tab Navigation, Chart.js, Modals, State)
├── README.md                     # เอกสารอธิบายโปรเจกต์
├── assets/                       # ไดเรกทอรีจัดเก็บสื่อและรูปภาพ
│   ├── images/                   # รูปภาพ Avatar, Project, Certificates
│   └── ...
└── scripts/                      # สคริปต์ยูทิลิตี้ภาษา Python
    ├── remove_background_auto.py # สคริปต์ลบแบ็คกราวด์อัตโนมัติ
    └── remove_background_final.py # สคริปต์ประมวลผลรูปภาพโปรไฟล์ฉบับสมบูรณ์
```

---

## 🚀 วิธีการใช้งาน (Getting Started)

### 1. เปิดใช้งานผ่านเว็บเบราว์เซอร์
เปิดไฟล์ `index.html` โดยตรงบนเว็บเบราว์เซอร์ หรือใช้งานผ่าน Live Server ใน VS Code / IDE ที่ใช้:
```bash
# หรือใช้ npx serve
npx serve .
```

### 2. การใช้งาน Python Background Removal Scripts (ถ้าต้องการ)
ติดตั้งไลบรารีที่จำเป็นก่อนรันสคริปต์ในโฟลเดอร์ `scripts/`:
```bash
pip install rembg pillow
```
รันสคริปต์เพื่อตัดขอบลบพื้นหลังภาพ Avatar:
```bash
python scripts/remove_background_final.py
```

---

## 🛠️ เทคโนโลยีที่ใช้ (Tech Stack)
- **Frontend Core**: HTML5, CSS3 (Vanilla CSS with Flexbox/Grid), JavaScript (ES6+)
- **Font**: Google Fonts (`Inter`, `Mitr`)
- **Libraries**: [Chart.js](https://www.chartjs.org/) (สำหรับกราฟสถิติทักษะ)
- **Python Tools**: Python 3.x, `rembg`, `Pillow` (PIL)

---

## 📝 License
โปรเจกต์นี้จัดทำขึ้นเพื่อการศึกษาและการจัดทำพอร์ตโฟลิโอดิจิทัล (Personal & Educational Project)
