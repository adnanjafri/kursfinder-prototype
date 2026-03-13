# kursfinder-prototype

# KursFinder 🟢

**Find certified prevention courses in Germany and automatically generate your health insurance reimbursement application.**

KursFinder helps German residents discover §20 SGB V certified Präventionskurse, understand exactly how much their Krankenkasse will reimburse, upload their Teilnahmebescheinigung, and generate a ready-to-submit PDF Erstattungsantrag — all in one place.

👉 **[Live Demo](https://adnanjafri.github.io/kursfinder-prototype)** ← replace with your GitHub Pages URL

---

## The Problem

Every German health insurer reimburses up to €300–500/year for certified prevention courses (yoga, back health, stress management, nutrition). But almost nobody claims it because:

- Finding which courses are actually certified is confusing
- Reimbursement rates vary wildly between insurers and regions
- The paperwork (Erstattungsantrag) is manual, paper-heavy, and intimidating

KursFinder solves all three.

---

## Features

### 🔍 Course Discovery
- Browse 8 certified Präventionskurse across 5 categories (Yoga, Rücken, Stress, Ernährung, Fitness)
- Filter by category and search by name or provider
- Each card shows the exact reimbursement amount for your specific insurer

### 🏥 Multi-Insurer Support
| Insurer | Rate | Max per Course | Max per Year |
|---|---|---|---|
| Techniker Krankenkasse (TK) | 80% | €150 | €300 |
| AOK Bayern | 100% | €150 | €300 |
| AOK Hessen | 100% | €150 | €300 |
| AOK NordWest | 80% | €250 | €500 |
| AOK Baden-Württemberg | 100% | €80 | €160 |
| AOK Niedersachsen | 100% | €100 | €200 |
| AOK Nordost | 100% | €150 | €300 |
| AOK Rheinland/Hamburg | 100% | €100 | €200 |

### 📄 Document Upload
- Upload Teilnahmebescheinigung as PDF or photo
- File preview before submission

### 📋 PDF Erstattungsantrag Generation
- Auto-generates a formal German reimbursement letter
- Pre-filled with user name, member number, course details, and insurer address
- Downloadable as a real PDF (via jsPDF)
- Simulated email submission to insurer

### 📊 Reimbursement Tracker
- Annual budget progress bar per insurer
- Per-course status: Neu → Bereit → Eingereicht
- Real-time remaining budget calculation

### 🧪 Demo Mode
Two one-click demos with pre-filled sample data:
- **🔵 TK Demo** — Laura Becker, 3 courses in different pipeline stages
- **🟢 AOK Demo** — Thomas Weiß (AOK NordWest), 3 courses in different pipeline stages

---

## Getting Started

### Option 1 — View live
Open the [GitHub Pages URL](https://adnanjafri.github.io/kursfinder-prototype) in any browser. No installation needed.

### Option 2 — Run locally
```bash
git clone https://github.com/yourusername/kursfinder-prototype.git
cd kursfinder-prototype
open index.html
```
No build step, no dependencies, no server required. Just open `index.html` in a browser.

---

## Project Structure

```
kursfinder-prototype/
└── index.html      # Entire app — HTML, CSS, and JS in one file
└── README.md       # This file
```

This is an intentionally simple single-file prototype. Everything lives in `index.html` to make sharing, testing, and iteration as frictionless as possible.

---

## How to Use

1. **Onboarding** — Enter your name, member number, and select your Krankenkasse (and AOK region if applicable)
2. **Discover** — Browse and filter certified courses; tap a card for full details and reimbursement breakdown
3. **Book** — Tap "Buchen" to add a course to your tracker
4. **Upload** — After completing the course, upload your Teilnahmebescheinigung
5. **Generate PDF** — KursFinder generates your Erstattungsantrag; download and submit to your insurer

Or tap **🔵 TK Demo** / **🟢 AOK Demo** on the start screen to skip onboarding and explore with sample data.

---

## Tech Stack

| | |
|---|---|
| **Frontend** | Vanilla HTML, CSS, JavaScript — no framework |
| **PDF Generation** | [jsPDF 2.5.1](https://github.com/parallax/jsPDF) via CDN |
| **Hosting** | GitHub Pages |
| **Data** | Static sample data (no backend) |

---

## Roadmap

This is a frontend prototype. Planned features for a production version:

- [ ] User authentication
- [ ] Real course database with live availability and booking
- [ ] Direct API integration with TK, AOK, and other Krankenkassen
- [ ] Automated Erstattungsantrag submission (no manual PDF upload)
- [ ] Push notifications for reimbursement status updates
- [ ] Support for additional insurers (Barmer, DAK, IKK, etc.)
- [ ] Location-based course search
- [ ] Document storage for past submissions

---

## Contributing

This project is in early prototype stage. Feedback and contributions welcome — open an issue or submit a pull request.

---

## Disclaimer

Reimbursement rates and limits are based on publicly available information as of early 2025 and may vary. Always confirm current rates directly with your Krankenkasse. This app does not submit documents to insurers on your behalf — the email submission feature is simulated for demo purposes only.

---

## License

MIT — free to use, modify, and distribute.
