# Cyber Security Base Project I
<br>
The application enables users to create accounts, log in, and share recipes with ingredients and instructions. Users can add, edit, delete, browse, and search recipes, categorize them, view their own contributions on a profile page, and leave comments and ratings, with each recipe displaying its feedback and average score.
<br>
<br>
This web application has CSRF vulnerability and 4 different flaws from the OWASP top ten list security flaws on purpose. The flaws are pointed out in the project and the steps to fix them are provided as well.
<br><br>

## Installation instructions
<br>

> [!IMPORTANT]
> Please make sure, that you have *Python3* installed.
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

**4. Install ```flask``` library:**
```bash
pip install flask
```
>[!NOTE]
>Uses SQLite with automatic initialization — no external database needed

**5. Create database:**
```bash
sqlite3 database.db < schema.sql
sqlite3 database.db < init.sql
```


**6. Execute flask-app:** <br>

Normal mode:
```bash
flask run
```

Debug mode (optional):
```bash
flask run --debug
```
<br>
