# Cyber Security Project I
<br>
This web application has 5 different flaws from the OWASP top ten list security flaws on purpose. The flaws are pointed out in the project and the steps to fix them are provided as well.
<br><br>

## Installation instructions
<br>

> [!IMPORTANT]
> Please make sure, that you have *python3* installed. The app is developed in Python 3.12.3
<br><br>

**1. Clone the repository:**
```bash
git clone https://github.com/hodelma/CSB-Project-I.git
```


**2. Create virtual environment (venv):**
```bash
python3 -m venv venv
```


**3. Enable venv:**
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


**6. Execute flask-app:**
```bash
flask run
```

**7. Executing the app in debug mode (optional):**
```bash
flask run --debug
```
<br>
