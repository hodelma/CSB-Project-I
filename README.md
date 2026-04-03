# Cyber Security Base Project I
<br>
The application enables users to create accounts, log in, and share recipes with ingredients and instructions. Users can add, edit, delete, browse and search recipes, categorize them, view their own contributions on a profile page and leave comments and ratings, with each recipe displaying its feedback and average score.
<br>
<br>
This web app has a CSRF vulnerability and 4 different flaws from the OWASP top ten list (2017) security flaws on purpose. The flaws are pointed out in the project and the steps to fix them are provided as well.
<br><br>

**The flaws I have chosen for this project:**
<br>
- Flaw 1: Cross-Site Request Forgery (CSRF)
- Flaw 2: A7:2017-Cross-Site Scripting (XSS)
- Flaw 3: A1:2017-Injection
- Flaw 4: A2:2017-Broken Authentication
- Flaw 5: A5:2017-Broken Access Control
<br><br>

## Installation instructions
<br>

> [!IMPORTANT]
> Please make sure, that you have *Python3* and python-dotenv package installed. If dotenv is not installed, follow step 4 regarding dotenv.
<br><br>

**1. Clone the repository:**
```bash
git clone https://github.com/hodelma/CSB-Project-I.git
cd CSB-Project-I
```


**2. Create a virtual environment (venv):**
```bash
python3 -m venv venv
```


**3. Activate venv:**
```bash
source venv/bin/activate
```

**4. Install ```flask``` library (and dotenv if not installed):**
```bash
pip install flask
pip install python-dotenv
```
>[!NOTE]
>Uses SQLite with automatic initialization — no external database needed

**5. Create database:**
```bash
sqlite3 database.db < schema.sql
sqlite3 database.db < init.sql
```

>[!TIP]
>Before running the Flask app, initialize and populate the database with seed data:
>```bash
>python seed.py


**6. Run flask-app:** <br>

Normal mode:
```bash
flask run
```

Debug mode (optional):
```bash
flask run --debug
```
<br>
