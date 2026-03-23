# Cyber Security Project I
This web application has 5 different flaws from the OWASP top ten list security flaws on purpose. The flaws are pointed out in the project and the steps to fix them are provided as well.
<br><br>
## Installation instructions
*Please, make sure, that you have python3 installed. The app is developed in Python 3.12.3*
<br><br>

The project operates with SQLite, so there is no need for setting up your own PostgreSQL or any other database. The db is initialized automatically.

1. Clone the repository:
```bash
git clone https://github.com/hodelma/Reseptisovellus.git
```


2. Create virtual environment (venv):
```bash
python3 -m venv venv
```


3. Enable venv:
```bash
source venv/bin/activate
```

4. Install ```flask``` library:
```bash
pip install flask
```


5. Create database:
```bash
sqlite3 database.db < schema.sql
sqlite3 database.db < init.sql
```


6. Execute flask-app:
```bash
flask run
```

7. Executing the app in debug mode (optional):
```bash
flask run --debug
```
<br>
