# 📚 Course Collision Checker

Check if returning students have already taken courses they're scheduled for.

---

## 👉 [START HERE → Open the Tool](https://adminswissedcol.github.io/collision-checker/)

**Everything happens in the tool — no need to open Google Sheets until viewing results!**

---

## How It Works

| Step | What You Do |
|------|-------------|
| **1** | Upload timetable PDF → Click "Send to Google Sheet" |
| **2** | Paste class list URL → Click "Import" |
| **3** | Click "Update Raw Data" *(required on first use)* |
| **4** | Click "Check for Collisions" → View Results |

That's it! All from one page. 🎉

---

## Understanding Results

| Row Color | Meaning |
|-----------|---------|
| 🟨 **Orange** | Total grade <60% — Insufficient, may need academic review |
| 🟥 **Light Red** | Total grade ≥60% — Passed, cannot retake course |
| ✅ **Green** | No collisions found |

**Grade Calculation:** The "Avg Grade" column shows the **SUM** of all "Contribution %" values for each student+course+session combination.

**Note:** A "collision" only counts if the student has **actual grades recorded** (non-empty "Contribution %"). Students enrolled but with no grades are NOT flagged.

## Filtering Results

**Quick Filters (easiest):**
Use the menu: **Collision Checker → Quick Filters** to instantly filter by:
- ⚠️ 0-59% (Insufficient)
- ✓ 60-100% (Passed)  
- Show All

**Manual Filtering:**
- Click any column header dropdown in row 4 to filter
- Create a **Filter View** (Data → Filter views) for reusable filters

The Results sheet also shows:
- **Metadata** (rows 1-3): Which PDF and class list were used
- **Filter buttons** (D1-G1): Visual reminder of available filters

---

## 🔗 Direct Links

| Resource | Link |
|----------|------|
| **🚀 Online Tool** | [adminswissedcol.github.io/collision-checker](https://adminswissedcol.github.io/collision-checker/) |
| **📊 Results Tab** | [View Results](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=808012596#gid=808012596) |

---

## 📋 Supported Levels

Certificate • Diploma • High Diploma • BBA • PGD • MBA • CUL I • CUL II • English

---

## 🛠️ Admin Setup

If setting up from scratch, see [`CollisionChecker.gs`](CollisionChecker.gs) for the Apps Script code.

**Important:** After updating the Apps Script, you must **re-deploy** the Web App:
1. Extensions → Apps Script → Deploy → Manage deployments
2. Edit → New version → Deploy

---

## 📁 Files

| File | Description |
|------|-------------|
| `index.html` | The online tool |
| `CollisionChecker.gs` | Google Apps Script |

---

*Swiss Educational College*
