# SkillBridge AI - AI Career Transition & Upskilling Agent

SkillBridge AI adalah agen kecerdasan buatan (AI Agent) yang dirancang untuk mengatasi tantangan perubahan industri dan kesenjangan keterampilan di era kecerdasan buatan. Solusi ini dikembangkan untuk kompetisi National Hackathon (Hacktiv8 x IBM SkillsBuild x Komdigi) pada tema **Education & Future of Work**.

---

## 📌 Problem Statement
Di era otomatisasi dan kemajuan AI, banyak mahasiswa, fresh graduate, dan profesional muda menghadapi ketidakpastian karier. Modul pelatihan tradisional cenderung generik (one-size-fits-all) dan tidak memetakan kesenjangan keterampilan (skill gap) secara riil terhadap kebutuhan industri terkini.

## 💡 Proposed Solution
SkillBridge AI memanfaatkan agen interaktif berbasis **Langflow** dan **IBM Granite/IBM Bob** untuk:
1. Menganalisis profil/CV pengguna terhadap target pekerjaan impian.
2. Mengkalkulasi Skill Match Score (0-100%) secara akurat.
3. Menyusun rencana belajar (Learning Roadmap) 4 minggu yang dipersonalisasi.
4. Merekomendasikan 3 proyek portofolio yang relevan dengan industri.

---

## 🛠️ Tech Stack & Architecture
- **Workflow Orchestration**: Langflow
- **LLM Engine**: IBM Granite / IBM watsonx.ai (via IBM Bob Integration)
- **Deployment**: Local Environment Execution

### Flow Workflow:
`[Chat Input: CV & Target Role]` ➡️ `[Prompt Template Engine]` ➡️ `[IBM Granite LLM Reasoning]` ➡️ `[Chat Output: Score, Gap, Roadmap & Projects]`

---

## 🚀 How to Run Locally

1. **Prerequisites**:
   - Python 3.10+
   - Langflow terinstal (`pip install langflow` atau Langflow Desktop App)

2. **Setup Instructions**:
   - Buka aplikasi Langflow atau jalankan perintah `langflow run` di terminal.
   - Pada halaman dashboard Langflow, pilih **Import**.
   - Unggah file `skillbrigde.json` yang ada pada repositori ini.
   - Buka flow tersebut, masukkan API Key IBM watsonx.ai / LLM yang sesuai pada node model.
   - Klik **Playground** dan jalankan pengujian dengan menginput CV serta target pekerjaan.

---

## ⚖️ Responsible AI Implementation
- **Fairness & Non-Bias**: Menganalisis berdasarkan bukti kompetensi, menghindari bias ras, gender, dan latar belakang non-akademis.
- **Privacy First**: Data profil pengguna hanya diproses secara lokal pada session aktif dan tidak disimpan untuk pelatihan ulang model umum.
- **Human Oversight**: Hasil roadmap berfungsi sebagai panduan, di mana kontrol keputusan akhir tetap ada di tangan pengguna.

---

## 📄 License
MIT License - Disusun untuk Hackathon Nasional 2026.
