# 📚 Course Collision Checker

Check if returning students have already taken courses they're scheduled for.

---

## 👉 [START HERE → Open the Tool](https://adminswissedcol.github.io/collision-checker/)

**Just follow the 4 steps in the tool — everything is explained there!**

---

## Quick Summary

1. **Upload** timetable PDF → extracts courses & levels
2. **Paste** courses into Google Sheet (pastes directly into columns!)
3. **Paste** class list (returning students)
4. **Click** "Check for Collisions" → see results

💡 **Raw data updates automatically** from nightly backups via menu: `Collision Checker → 🔄 Update Raw Data`

---

## 🔗 Direct Links

| Resource | Link |
|----------|------|
| **🚀 Online Tool** | [adminswissedcol.github.io/collision-checker](https://adminswissedcol.github.io/collision-checker/) |
| **📊 Google Sheet** | [Open Spreadsheet](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit) |

### Sheet Tabs
- [Return](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=519500099#gid=519500099) — Paste class list here
- [Courses](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=1675119560#gid=1675119560) — Course codes & levels
- [Students](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=980436297#gid=980436297) — Auto-populated
- [Results](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=808012596#gid=808012596) — Collision results

---

## 📋 Supported Levels

Certificate • Diploma • High Diploma • BBA • PGD • MBA • CUL I • CUL II • English

---

## 🛠️ Admin: Setting Up a New Spreadsheet

1. Create a sheet named `raw` with historical grade data (needs `Email` and `Course Code` columns)
2. Go to **Extensions → Apps Script**
3. Paste the code from [`CollisionChecker.gs`](CollisionChecker.gs)
4. Save and refresh
5. Click **Collision Checker → Setup All Sheets**

---

## 📁 Files

| File | Description |
|------|-------------|
| `index.html` | The online tool (PDF extractor + instructions) |
| `CollisionChecker.gs` | Google Apps Script code |

---

*Swiss Educational College*
