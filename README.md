# SeleniumWebdriver-python-pytest-framework
The development of Selenium Webdriver python pytest framework

## Installation steps

That is the safest and most important preparation for your Optimworks interview because the JD specifically mentions:

* Selenium
* Automation framework
* Python
* Regression automation
* End-to-end testing



# Recommended Interview Preparation Order

## Phase 1 — Core Selenium Framework (Priority)

Focus on:

### Mandatory Setup

1. Git
2. Python
3. VS Code
4. Virtual Environment
5. Selenium
6. PyTest
7. WebDriver Manager

---

# Minimal Enterprise Setup (Recommended)

## STEP 1 — Clone Repository

```bash id="5m8v2q"
git clone https://github.com/prasad-04t/SeleniumWebdriver-python-pytest-framework.git
```

```bash id="1x7p4n"
cd SeleniumWebdriver-python-pytest-framework
```

---

# STEP 2 — Install Python

Download:

[Python Downloads](https://www.python.org/downloads/?utm_source=chatgpt.com)

IMPORTANT:
✅ Check:

```text id="8v5n2m"
Add Python to PATH
```

---

# STEP 3 — Verify Python

```bash id="3q7m1x"
python --version
```

```bash id="9n4v2p"
pip --version
```

---

# STEP 4 — Install VS Code

[Visual Studio Code](https://code.visualstudio.com/?utm_source=chatgpt.com)

Install extension:

* Python

---

# STEP 5 — Open Project

```bash id="7x2m5q"
code .
```

---

# STEP 6 — Create Virtual Environment

```bash id="2p8n4v"
python -m venv venv
```

---

# STEP 7 — Activate Virtual Environment

## Windows

```bash id="5v1m9q"
venv\Scripts\activate
```

Expected:

```text id="4x7p2n"
(venv)
```

---

# STEP 8 — Install Selenium

```bash id="9m2v5q"
pip install selenium
```

---

# STEP 9 — Install PyTest

```bash id="6q8x1n"
pip install pytest
```

---

# STEP 10 — Install WebDriver Manager

```bash id="1v5m8p"
pip install webdriver-manager
```

This automatically manages ChromeDriver versions.

---

# STEP 11 — Create Enterprise Folder Structure

Inside project:

```text id="7m2x5v"
project/
│
├── tests/
├── pages/
├── utils/
├── reports/
├── screenshots/
├── requirements.txt
```

---

# STEP 12 — Create First Selenium Test

Create file:

```text id="2n8v4p"
tests/test_google.py
```

Code:

```python id="5x1m7q"
from selenium import webdriver
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager

def test_google():
    driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()))
    
    driver.get("https://www.google.com")
    
    assert "Google" in driver.title
    
    driver.quit()
```

---

# STEP 13 — Run Test

```bash id="8p2m5v"
pytest
```

Expected:

```text id="4v7n1x"
1 passed
```

---

# STEP 14 — Create requirements.txt

```bash id="9x5m2q"
pip freeze > requirements.txt
```

---

# STEP 15 — Push Code to GitHub

```bash id="6m1v8p"
git add .
```

```bash id="2x7q5n"
git commit -m "Initial Selenium PyTest framework"
```

```bash id="5p8m1v"
git push
```

---

# What You’ll Learn Next

After Selenium setup:

1. PyTest fixtures
2. Page Object Model (POM)
3. Explicit waits
4. Locators
5. Dropdown handling
6. Frames/windows
7. Data-driven testing
8. HTML reports
9. Logging
10. Jenkins integration

This is exactly how enterprise automation frameworks are built.


