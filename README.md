# 📚 Course Collision Checker

Check if returning students have already taken courses they're scheduled for.

---

## 👉 [START HERE → Open the Tool](https://adminswissedcol.github.io/collision-checker/)

**Just follow the 4 steps in the tool — everything is explained there!**

---

## Quick Summary

1. **Upload** timetable PDF → extracts courses & levels
2. **Click "Send to Google Sheet"** → courses imported automatically!
3. **Import students** via URL (no copy-paste needed!)
4. **Click** "Check for Collisions" → see results

💡 **Raw data updates** from nightly backups: `Collision Checker → 🔄 Update Raw Data`

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
6. Deploy as Web App: **Deploy → New deployment → Web app → Anyone can access**
7. Update the `WEB_APP_URL` in `index.html` if the deployment URL changes

---

## 📁 Files

| File | Description |
|------|-------------|
| `index.html` | The online tool (PDF extractor + instructions) |
| `CollisionChecker.gs` | Google Apps Script code |

---

*Swiss Educational College*
