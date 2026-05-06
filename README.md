# IT23228108_TESTCASES-IT3040_ITPM

# Singlish to Sinhala Transliteration Testing Automation

## 📌 Project Overview
This project automates the testing process of a Singlish-to-Sinhala transliteration web application using Python and Playwright.  
The system reads test cases from an Excel file, automatically enters the input text into the web application, captures the generated Sinhala output, compares it with the expected output, and updates the Excel sheet with the actual results and test status (PASS/FAIL).

---

# 🚀 Features
- Automated browser interaction using Playwright
- Reads test cases from Excel files
- Supports Singlish to Sinhala transliteration testing
- Automatically captures actual output
- Compares expected and actual outputs
- Updates PASS/FAIL status automatically
- Supports retry handling and configurable wait times
- Frontend-only automation testing

---

# 🛠️ Technologies Used
- Python 3
- Playwright
- OpenPyXL
- Excel (.xlsx)

---

# 📂 Project Structure

```text
IT23228108/
│
└── test_automation/
    │
    └── test_automation/
        │
        ├── .git/
        ├── IT23228108.xlsx
        ├── README.md
        ├── test_automation.py
        └── IT23228108.txt
```

---

# ⚙️ Installation Guide

## 1️⃣ Install Python
Download and install Python:

https://www.python.org/downloads/

✔ Make sure to enable:

```text
Add Python to PATH
```

---

# 2️⃣ Verify Python Installation

```bash
python --version
```

---

# 3️⃣ Install Required Packages

```bash
pip install playwright openpyxl
```

---

# 4️⃣ Install Playwright Browsers

```bash
python -m playwright install
```

---

# ▶️ How to Run the Project

## Step 1
Open terminal / CMD inside the project folder:

```text
IT23228108/test_automation/test_automation
```

---

## Step 2
Run the following command:

```bash
python test_automation.py --excel "IT23228108.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 4000 --type-delay-ms 30 --slow-mo-ms 200 --save-every 1
```

---

# ⚡ Alternative Fast Mode

```bash
python test_automation.py --excel "IT23228108.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 2000 --type-delay-ms 10 --slow-mo-ms 0 --save-every 1 --headless
```

---

# 📊 Excel File Format

| Input | Expected Output | Actual Output | Status |
|------|----------------|---------------|--------|

---

# 🧪 Test Case Details

- Total Test Cases: 50+
- Test Type: Negative Testing
- Includes:
  - Invalid Singlish inputs
  - Abbreviations
  - Slang words
  - Misspelled text
  - Mixed English/Sinhala inputs
  - UI/API failure scenarios
  - Question-type inputs
  - Distorted transliteration patterns

---

# ✅ Output
After execution:

- Actual Sinhala outputs are automatically saved
- PASS/FAIL status is updated in Excel
- Results are stored directly in the Excel file

---

# 📌 Sample Test Case

| Input | Expected Output |
|------|----------------|
| mata exam ekata study karanna ona | මට exam එකට study කරන්න ඕන |

---

# ❗ Common Errors and Fixes

## 1️⃣ File Not Found Error

### Error:
```text
File not found
```

### Fix:
Make sure the Excel file is inside the same project folder.

---

## 2️⃣ Permission Denied Error

### Error:
```text
Permission denied
```

### Fix:
Close the Excel file before running the automation.

---

## 3️⃣ Failed to Fetch Error

### Reason:
- Internet issue
- Website/API issue
- Slow server response

### Fix:
Use slower timing values:

```bash
python test_automation.py --excel "IT23228108.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 4000 --type-delay-ms 30 --slow-mo-ms 200 --save-every 1
```

---

## 4️⃣ Browser Closed Error

### Fix:
Reinstall Playwright browsers:

```bash
python -m playwright install
```

---

# 🎯 Purpose of the Project
The main purpose of this project is to automate transliteration testing and identify:
- Incorrect Sinhala conversions
- UI/API failures
- Transliteration mismatches
- Automation testing issues

---

# 👩‍💻 Author

### Sandani Nehansa Wijesinghe
Undergraduate | Information Technology & Software Engineering  
SLIIT University

---

# 🔗 GitHub Repository
Upload this project to GitHub and include:
- Source code
- Excel test cases
- README.md
- Required files

---

# ✅ Final Notes
- Keep the Excel file closed while running the automation
- Use stable internet connection
- Do not rename project files while the script is running
- Use Python 3.11 or 3.12 for best Playwright compatibility
