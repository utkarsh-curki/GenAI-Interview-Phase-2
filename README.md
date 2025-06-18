# GenAI-Interview-Phase-2

# ✅ **Updated GenAI Internship Assignment**

### **Stage: Data Extraction Only**

---

## 📌 Objective

To **extract structured and meaningful data** from the **given Excel source file**, which may include multiple sheets and hierarchical tables. Your goal is to convert this into a **clean, structured JSON format**, suitable for downstream AI processing and future template population.

---

## 🧠 Task Overview

You are given:

* **1 Excel file (Template data)** — may have multiple sheets with different formats
* **Source Data** - Containing multiple source data
* Your job is to extract structured information sheet-by-sheet and represent it in **modular JSON format**

---

## 🛠️ Instructions

1. **Inspect** the Excel file carefully.
2. **Understand** the structure, headers, and data intent in each sheet (some may have nested tables, merged cells, or multi-row headers).
3. **Design a JSON schema** for each sheet to reflect its structure and business meaning (e.g., clients, hours worked, funding types).
4. **Extract** the data from each sheet and populate it into the corresponding JSON structure.
5. Ensure:

   * No data loss
   * Proper type conversion (e.g., numbers, strings)
   * Keys are meaningful
   * You preserve the hierarchy or relationships present in the tables

---

## ✅ Expected Output

Your output should be a Python or JSON file (or both) that:

* Contains **structured JSON data** extracted from the source Excel file
* Follows **one JSON structure per sheet**
* Has **clean field names**, removing whitespace and clarifying ambiguous headers
* Handles **empty cells or merged fields** gracefully

### Example Output

```json
{
  "WAGES": [
    {
      "role": "Registered nurses",
      "hours": {
        "week1": 24,
        "week2": 30,
        "week3": 28,
        "week4": 25
      }
    },
    ...
  ],
  "INCOME_BY_SERVICE": [
    {
      "service": "HCP Level 1",
      "week_costs": {
        "week1": 1200,
        "week2": 1250,
        "week3": 1300,
        "week4": 1350
      }
    },
    ...
  ]
}
```

---

## 📦 Deliverables

Your `.zip` file should include:

* ✅ `extract.py`: Code that reads the Excel and outputs structured JSON
* ✅ `extracted_data.json`: Output JSON file
* ✅ `README.md` with:

  * Your approach to schema design
  * Any assumptions made (e.g., how you handled merged cells, multiple header rows, etc.)
  * Instructions to run the code (`pip install`, etc.)

---

## ✅ Submission

* Create a **public GitHub repository** with:

  * Code
  * `requirements.txt`
  * Output JSON
  * README
* Email the GitHub link to **[utkarsh@curki.ai](mailto:utkarsh@curki.ai)**
