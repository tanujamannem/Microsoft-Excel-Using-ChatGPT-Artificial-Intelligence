## 🧩 Flash Fill in Excel — Quick Notes

**Flash Fill** automatically recognizes patterns in your data and fills values — perfect for quick, no-formula data transformations.

### ⚙️ How to Use
- **Smart Tag:** Type first result → drag down → choose *Flash Fill* from ⚙️ icon.  
- **Auto Pattern:** Start typing next value; Excel predicts rest → press **Enter**.  
- **Shortcut:** Press **Ctrl + E** or go to *Data → Flash Fill*.

### 🧠 Examples
- Extract first names → `Ian Turner → Ian`  
- Reverse names → `Ian Turner → Turner, Ian`  
- Extract text between slashes → `/THG/ → THG`  
- Change text case → `blue → Blue`  
- Fix errors → correct one cell → others auto-update

### 💡 Notes
- Works on **patterns**, not formulas  
- Doesn’t auto-refresh if source changes  
- Works in both **tables and ranges**  
- Best shortcut: **Ctrl + E**

**✅ Flash Fill = Fast, Simple, No-Code automation for Excel.**


## 🧮 Formula by Example — Quick Notes

**Formula by Example** (Excel Online only) automatically writes formulas from your examples — just like Flash Fill, but dynamic and auto-updating.

### ⚙️ Highlights
- Type 2–3 sample outputs in a **table column**, Excel detects the pattern and suggests a formula.  
- Click **Show Formula** → see the generated logic (e.g., `LEFT`, `FIND`, `TEXT`, `SUBSTITUTE`).  
- Click **Apply** → Excel fills the entire column with that formula.  
- Updates automatically when data changes.

### 🧠 Examples
- Extract first name → `Ian Turner → Ian`  
- Reverse names → `Ian Turner → Turner, Ian`  
- Extract codes → `/AB123/ → AB123`  
- Convert dates → `06/05/2025 → June`  
- Change case → `blue → Blue`

**💡 Notes:**  
Only available in **Excel Online** and works on **tables**. Uses standard Excel formulas for compatibility.  
**✅ Formula by Example = Flash Fill + Automation.**


## 🔠 Column from Examples — Power Query Quick Notes

**Column from Examples** is an AI-assisted feature in **Power Query** that lets Excel automatically write **M code** (Power Query formulas) based on the examples you provide.  
It’s similar to *Flash Fill*, but much more powerful — it generates reusable code that updates when your data changes.

### ⚙️ How It Works
1. Load your data into **Power Query** (`Data → From Table/Range`).
2. Go to **Add Column → Column from Examples** → choose *From All Columns* or *From Selection*.
3. Type 1–2 example results — Power Query detects the pattern and writes the code.
4. Click **OK** to apply and create a new calculated column.

---

### 🧠 Example 1 – Format Names
**Goal:** Convert `"Anders, Maria"` → `"M Anders"`  
- Type `M Anders` and `A Hello` for next rows.  
- Power Query writes the formula using:  
  `Text.Combine` + `Text.BeforeDelimiter` + `Text.AfterDelimiter`  
- Result: Creates new “Student Name” column automatically.

---

### 🧮 Example 2 – Categorize Scores
**Goal:** Convert numeric scores into grades.  
- Example logic:  
  - ≥ 90 → Distinction  
  - ≥ 80 → Merit  
  - ≥ 65 → Pass  
  - Else → Fail  
- Column from Examples writes a **nested IF structure** automatically in M code.  
- You can then tweak thresholds or rename the column (e.g., `Grade`).

---

### 💡 Notes
- Works inside **Power Query**, not the main Excel grid.  
- Creates **M code**, not formulas — great for automation and data transformation.  
- Excellent for users new to Power Query who want Excel to **auto-write logic**.  
- Helps connect and transform **external data sources** before loading back to Excel.

**✅ Column from Examples = Flash Fill + Formula by Example + Power Query Automation.**

