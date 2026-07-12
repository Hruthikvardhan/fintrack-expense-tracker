# 💰 FinTrack — Personal Expense Tracker

<div align="center">

![FinTrack Banner](https://img.shields.io/badge/FinTrack-Personal%20Finance%20Tracker-f6c90e?style=for-the-badge&logo=bitcoin&logoColor=black)

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20App-48bb78?style=for-the-badge&logo=vercel&logoColor=white)](https://fintrack-expense-tracker-flax.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-Hruthikvardhan-63b3ed?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Hruthikvardhan/fintrack-expense-tracker)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)](https://www.chartjs.org/)

**A fully responsive personal finance tracker built with pure HTML, CSS & Vanilla JavaScript.**
**No frameworks. No backend. No database. Just clean code.**

[🚀 Live Demo](https://fintrack-expense-tracker-flax.vercel.app/) · [🐛 Report Bug](https://github.com/Hruthikvardhan/fintrack-expense-tracker/issues) · [✨ Request Feature](https://github.com/Hruthikvardhan/fintrack-expense-tracker/issues)

</div>

---

## 📸 Preview

> 🌙 Dark Mode — Clean, modern UI with smooth animations

```
+------------------+----------------------------------------+
|  💰 FinTrack     |  Dashboard          [Export] [+ Add]  |
|                  |----------------------------------------|
|  📊 Dashboard ●  |  [Balance ₹46,522] [Income] [Expense] |
|  ➕ Add          |  [====Progress Bar=====]  45%          |
|  📋 History      |  [Recent Tx]    [Top Categories]       |
|  📈 Analytics    |                                        |
|  🎯 Budget       |                                        |
|                  |                                        |
|  [⬇ Export CSV] |                                        |
|  [🌙 Dark Mode] |                                        |
+------------------+----------------------------------------+
```

---

## ✨ Features

### 📊 Dashboard

- **Total Balance** — real-time income minus expenses
- **Income & Expense Cards** — with transaction counts
- **Spending Progress Bar** — visual % of budget used
- **Color coded** — Green (safe), Orange (80%), Red (exceeded)
- **Recent Transactions** — last 5 at a glance
- **Top Expense Categories** — with mini progress bars

### ➕ Add Transaction

- Income / Expense **type toggle**
- Fields — Name, Amount, Date, Category
- **10 categories** — Salary, Freelance, Food, Transport, Shopping, Entertainment, Bills, Health, Education, Other
- **Full form validation** — no empty fields, no negative amounts
- **Success toast** on submit + auto navigate to dashboard

### 📋 Transaction History

- All transactions listed **newest first**
- **Search** by name or category
- **Filter** by category, type, date range
- **Edit** — modal popup with pre-filled data
- **Delete** — with confirmation dialog
- **Clear All** — wipe all data at once

### 📈 Analytics

- **Doughnut Chart** — expense breakdown by category
- **Bar Chart** — last 6 months income vs expense
- Powered by **Chart.js 4.4.0**
- Charts **adapt** to dark and light mode

### 🎯 Budget Goals

- Set **monthly budget limit**
- Tracks **current month expenses only**
- Shows remaining budget and % used
- **⚠️ Warning** at 80% usage
- **🚨 Alert** when budget exceeded

### 🌙 Dark / Light Mode

- Toggle between dark and light theme
- **Persists** after page refresh
- Smooth **0.3s transition** between themes

### ⬇️ Export CSV

- Export all transactions as **CSV file**
- Auto named — `fintrack-YYYY-MM-DD.csv`
- Opens in Excel or Google Sheets

---

## 🛠️ Built With

| Technology             | Purpose                                |
| ---------------------- | -------------------------------------- |
| **HTML5**              | Structure and semantic markup          |
| **CSS3**               | Styling, animations, responsive layout |
| **Vanilla JavaScript** | Logic, CRUD, DOM manipulation          |
| **Chart.js 4.4.0**     | Pie and bar chart rendering            |
| **Google Fonts**       | Syne (display) + DM Sans (body)        |
| **localStorage**       | Client-side data persistence           |
| **Vercel**             | Deployment and hosting                 |

> ❌ No React · No Angular · No Vue · No Bootstrap · No jQuery · No Backend · No Database

---

## 🚀 Getting Started

### Option 1 — Direct Open (Easiest)

```bash
# Just download and open in browser
# No installation needed!
open expense-tracker.html
```

### Option 2 — Clone Repository

```bash
# Clone the repo
git clone https://github.com/Hruthikvardhan/fintrack-expense-tracker.git

# Navigate to folder
cd fintrack-expense-tracker

# Open in browser
open expense-tracker.html
# OR double click the file in file explorer
```

> ✅ No npm install · No build step · No server needed

---

## 📁 Project Structure

```
fintrack-expense-tracker/
│
├── 📄 expense-tracker.html    # Entire application (HTML + CSS + JS)
└── 📄 README.md               # Project documentation
```

> Single file architecture — HTML, CSS and JavaScript all in one file.

---

## 🎯 How It Works

### Single Page Application (SPA)

```
All 5 sections exist in HTML simultaneously
CSS hides them with display: none
JavaScript shows active section with display: block
No page reloads — instant navigation ✅
```

### Data Flow

```
User Action → JavaScript Function → Update Array → Save to localStorage → Re-render UI
```

### localStorage Keys

```javascript
ft_transactions; // Array of all transactions (JSON)
ft_budget; // Monthly budget limit (Number)
ft_theme; // dark or light (String)
ft_seeded; // First visit flag (String)
```

---

## 📱 Responsive Design

| Screen            | Layout                    |
| ----------------- | ------------------------- |
| Desktop (1280px+) | Sidebar + 3 column cards  |
| Tablet (900px)    | Sidebar + 2 column cards  |
| Mobile (720px-)   | Hamburger menu + 1 column |

---

## 🧪 Testing

Manually tested on:

- ✅ Google Chrome
- ✅ Microsoft Edge

Test cases covered:

- ✅ CRUD operations
- ✅ Form validation (empty, negative, zero)
- ✅ Budget warning at 80%
- ✅ Budget alert at 100%
- ✅ Dark / Light mode toggle
- ✅ CSV export
- ✅ Mobile responsive layout
- ✅ Data persistence after refresh

---

## 📚 JavaScript Concepts Used

```javascript
// DOM Manipulation
document.getElementById()
document.querySelectorAll()
element.classList.add/remove/toggle()
element.innerHTML / textContent

// Array Methods
.filter() .map() .reduce() .find()
.forEach() .sort() .slice() .unshift()

// localStorage
JSON.stringify() / JSON.parse()
localStorage.setItem() / getItem()

// Browser APIs
new Blob() / URL.createObjectURL()  // CSV export
setTimeout()                         // Toast auto-remove
confirm()                            // Delete confirmation
getComputedStyle()                   // Read CSS variables

// ES6+ Features
Arrow functions, Template literals
Destructuring, Spread operator
Default parameters, Ternary operator
```

---

## 🔮 Future Enhancements

- [ ] User authentication (Login / Register)
- [ ] Backend API with Node.js + Express
- [ ] Database integration (MongoDB / PostgreSQL)
- [ ] Recurring transactions
- [ ] PDF export
- [ ] Multi-currency support
- [ ] PWA (Progressive Web App)
- [ ] Email budget reports
- [ ] Bank statement import

---

## 👨‍💻 Developer

<div align="center">

**Hruthik Vardhan**
4th Year Engineering Student — GPCET

[![GitHub](https://img.shields.io/badge/GitHub-Hruthikvardhan-181717?style=for-the-badge&logo=github)](https://github.com/Hruthikvardhan)

_Built independently — No team, No mentor_
_Self-driven project — Planned, Designed, Developed, Tested and Deployed solo_

</div>

---

## 📄 License

```
MIT License — Free to use, modify and distribute
```

---

<div align="center">

**⭐ If you found this project helpful, please give it a star!**

Made with ❤️ by [Hruthik Vardhan](https://github.com/Hruthikvardhan)

</div>
