<div align="center">
  <img src="https://img.icons8.com/color/96/000000/exam.png" alt="Logo" width="80"/>
  <h1>🚀 Chhatro Bondhu Exam Portal</h1>
  <p>
    <b>A Full-Featured Cloud-Powered Online Examination Platform</b>
  </p>
  <p>
    Simulating real-world competitive exams like JEE/GATE with precision, real-time cloud sync, and complete admin control — powered by Firebase.
  </p>
  <p>
    <a href="#-features">Features</a> •
    <a href="#-preview">Preview</a> •
    <a href="#%EF%B8%8F-tech-stack--architecture">Tech Stack</a> •
    <a href="#%EF%B8%8F-setup--run">Quick Start</a>
  </p>
</div>

---

## 🏆 Project Highlights

- 🎯 **Real Exam Environment:** True-to-life simulation of JEE & GATE exam patterns.
- ☁️ **Firebase Cloud Backend:** Real-time data sync across all devices via Firebase Realtime Database.
- 🔒 **Firebase Authentication:** Secure Email/Password auth with persistent sessions — no more data loss on browser clear.
- 🖼️ **Rich Media Support:** Upload and store high-quality diagrams/images for questions, options, and solutions.
- 📊 **Performance Analytics:** Instant, detailed result breakdowns and real-time accuracy calculation.
- 🔐 **Role-Based Access Control:** Distinct, secure panels for Students and Administrators.
- 📱 **Mobile-Optimized & Responsive:** Carefully crafted UI to ensure mathematical equations and layouts scale flawlessly on mobile devices.

---

## 🖼️ Preview

<details open>
<summary><b>View Interface Screenshots</b></summary>
<br>

| 🔐 Login Interface | 🛠️ Admin Dashboard |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/569a3aff-df84-497a-bc1e-9d7dc0d2d215" width="400"/> | <img src="https://github.com/user-attachments/assets/9442eaa3-0830-4c18-a43c-6ffebde75b33" width="400"/> |

| 🎓 Student Dashboard | 📝 Exam Interface |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/6cee761d-dcc0-4f1a-9677-49f3f10d576a" width="400"/> | <img src="https://github.com/user-attachments/assets/9d025053-56f9-475c-8b45-2ce239e2b424" width="400"/> |

</details>

---

## ✨ Comprehensive Feature Set

### 👨‍🎓 For Students
- **Frictionless Onboarding:** Secure registration and login via Firebase Authentication with persistent sessions.
- **Dynamic Assessments:** Support for Multiple Choice (MCQ), Multiple Select (MSQ), and Numerical Input.
- **Precision Time Management:** Real-time countdown timer with automated warnings and critical state alerts.
- **Navigation Palette:** Quickly jump between questions, mark for review, and track answered vs. unanswered states.
- **Post-Exam Analytics:** Dive deep into performance metrics, time spent per question, and comprehensive answer keys.

### 👨‍🏫 For Administrators
- **Exam Management Suite:** Create, edit, and organize exams with customizable durations and instructions.
- **Advanced Question Editor:** 
  - Full LaTeX support for complex mathematical equations.
  - Image upload capabilities for questions, options, and step-by-step solutions.
- **Student Oversight:** Monitor registered students, track their attempts, and analyze overall results.
- **Flexible Marking Schemes:** Define custom positive/negative marking rules per question type.

---

## 🧠 Advanced Exam Engine

The core engine is built to handle the complexities of competitive testing:
- **Modular Sections:** Group questions by subjects (e.g., Physics, Chemistry, Mathematics).
- **Smart Status Tracking:** Real-time color-coded mapping (Answered, Unanswered, Marked for Review).
- **Nuanced Evaluation:**
  - **MCQ:** Standard positive/negative marking.
  - **MSQ:** Support for partial marking schemes.
  - **Numerical:** Precision floating-point validation with built-in ±0.5% error tolerance.

---

## 🛠️ Tech Stack & Architecture

This project is a masterclass in **Cloud-Powered Single-Page Web Development**. 

| Technology | Purpose |
| :--- | :--- |
| **React (via CDN)** | Component-based UI and complex state management. |
| **Babel** | In-browser JSX compilation. |
| **Firebase Realtime Database** | Cloud-hosted NoSQL database with real-time sync across all clients. |
| **Firebase Authentication** | Secure Email/Password auth with persistent sessions. |
| **KaTeX** | Lightning-fast, professional mathematical equation rendering. |
| **Vanilla CSS3** | Custom-built, responsive styling without heavy frameworks. |

### 🔒 Security Architecture

The database is secured with Firebase Security Rules that require authentication for all read/write operations:

```json
{
  "rules": {
    "users": { ".read": "auth != null", ".write": "auth != null" },
    "exams": { ".read": "auth != null", ".write": "auth != null" },
    "questions": { ".read": "auth != null", ".write": "auth != null" },
    "attempts": { ".read": "auth != null", ".write": "auth != null" },
    "malpractice_logs": { ".read": "auth != null", ".write": "auth != null" },
    "files": { ".read": "auth != null", ".write": "auth != null" }
  }
}
```

Mobile numbers are mapped to synthetic emails (e.g., `917003902225@exam.chhatrobondhu.app`) so users still log in with their mobile number and password — Firebase Auth runs silently underneath.

---

## ⚙️ Setup & Run

Getting started is incredibly simple—no `npm install` or servers required.

```bash
# 1. Clone the repository
git clone https://github.com/Swatadru/exam-portal.git

# 2. Navigate to the project directory
cd exam-portal

# 3. Launch the portal
# Simply open index.html in your favorite modern web browser
```

---

## 📊 Why This Project Stands Out

- **Cloud-First Architecture:** All data syncs in real-time via Firebase — accessible from any device, anytime.
- **Secure by Default:** Firebase Authentication + database security rules ensure only authenticated users can access data.
- **Session Persistence:** Users stay logged in across page refreshes and browser restarts.
- **High-Fidelity UI/UX:** A polished, modern interface that rivals commercial examination platforms.
- **Accessibility & Responsiveness:** Fluid typography and math rendering that adapts seamlessly from desktop to mobile.
- **Production-Ready Frontend:** Demonstrates advanced React patterns (stale closures prevention, efficient re-rendering, and asynchronous data handling).

---

## 🚀 Future Enhancements

- [x] **Cloud Synchronization:** Firebase Realtime Database for real-time sync across all devices. ✅
- [x] **Firebase Authentication:** Secure login with persistent sessions. ✅
- [ ] **Leaderboard System:** Global ranking among peers.
- [ ] **Progressive Web App (PWA):** Installable offline mode for students with limited internet access.
- [ ] **Export Capabilities:** Export results and question papers to PDF/CSV.

---

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<div align="center">
  <b>Built with ❤️ by Swatadru Paul</b><br>
  <i>Aspiring Software Development Engineer 🚀</i><br><br>
  
  If you found this project helpful or inspiring, please consider giving it a ⭐!
</div>
