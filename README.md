# 📚 Course Collision Checker

A tool to check if returning students have already taken courses they're scheduled for in the upcoming semester.

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| **PDF Course Extractor** | [Use Online Tool](https://adminswissedcol.github.io/course-collision-checker/) |
| **Google Sheet** | [Open Spreadsheet](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit) |

### Sheet Tabs
- [Return](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=519500099#gid=519500099) - Paste upcoming semester students here
- [Courses](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=1675119560#gid=1675119560) - Course codes mapped to levels
- [Students](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=980436297#gid=980436297) - Auto-populated from Return sheet
- [Results](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=808012596#gid=808012596) - Collision results

---

## 🚀 How to Use

### Step 1: Set Up Courses (one-time per semester)

1. Export your timetable as PDF from aSc Timetables
2. Go to the [PDF Course Extractor](https://adminswissedcol.github.io/course-collision-checker/)
3. Upload the PDF → courses are extracted automatically
4. Click **Copy to Clipboard**
5. Go to the [Courses tab](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=1675119560#gid=1675119560)
6. Select cell A2 and paste (Ctrl+V)

### Step 2: Check for Collisions

1. Paste your class list into the [Return tab](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=519500099#gid=519500099)
   - Must have columns: `Class` (with level like "26-T1-Class-Certificate") and `School Email`
2. Click menu: **Collision Checker → Check for Collisions**
3. View results in the [Results tab](https://docs.google.com/spreadsheets/d/1omcWpajVrVMTWiOdKL5YQr40KxlRHCogJpfKuRUsdWY/edit?gid=808012596#gid=808012596)

That's it! The script automatically imports students from Return and checks against historical data.

---

## 📋 Supported Levels

- Certificate
- Diploma
- High Diploma
- BBA
- PGD
- MBA
- CUL I
- CUL II
- English

---

## 🛠️ Setup (for new spreadsheet)

If setting up a fresh spreadsheet:

1. Create a sheet named `raw` with historical grade data (must have `Email` and `Course Code` columns)
2. Go to **Extensions → Apps Script**
3. Paste the code from `CollisionChecker.gs` in this repo
4. Save and refresh the spreadsheet
5. Click **Collision Checker → Setup All Sheets**

---

## 📁 Files in This Repo

| File | Description |
|------|-------------|
| `index.html` | PDF Course Extractor (runs in browser) |
| `CollisionChecker.gs` | Google Apps Script for the spreadsheet |
| `README.md` | This file |

---

## ❓ Troubleshooting

**"raw" sheet not found**
- Make sure your historical data tab is named exactly `raw`

**No collisions found but expected some**
- Check that course codes match exactly (e.g., `2040A` vs `2040B`)
- Verify student emails are identical in both Return and raw sheets

**PDF extraction missing course names**
- Course codes are reliably extracted; names sometimes need manual entry
- The collision checker only uses course codes, so missing names don't affect functionality

---

## 📝 License

Internal tool for Swiss Educational College
