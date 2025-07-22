# 🔣 Snippets

A collection of useful code fragments that can be reused in many projects.

---

## 🧪 Flask – JSON response helper

```python
from flask import jsonify

def response_json(msg, status=200):
    return jsonify({"message": msg}), status
```

---

## 🛠️ SQLAlchemy – initialize database

```python
from app import db
db.create_all()
```

---

## 🔒 JWT – generate token using pyjwt

```python
import jwt
import datetime

def generate_token(user_id, secret, expire_minutes=60):
    payload = {
        "sub": user_id,
        "exp": datetime.datetime.utcnow() + datetime.timedelta(minutes=expire_minutes)
    }
    return jwt.encode(payload, secret, algorithm="HS256")
```

---

## 🧹 Git – undo last commit (local)

```bash
git reset --soft HEAD~1
```

---

## 🔁 Git – interactive rebase

```bash
git rebase -i HEAD~3
```

---

## 🧪 Pytest – sample login test

```python
def test_login_valid(client):
    response = client.post("/login", json={"username": "admin", "password": "1234"})
    assert response.status_code == 200
    assert "token" in response.json
```
