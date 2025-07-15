# 🚀 How to Run IPL-ProScore on Any Computer

This guide will help you clone and run the IPL Score Prediction app using Python and Flask.

---

## ✅ Prerequisites

- Python 3.10+ (Python 3.11+ may need updated packages)
- Git
- A code editor (e.g., VS Code or Notepad++)
- Internet connection (to install dependencies)

---

## 🧱 Step 1: Clone the Repository

```bash
git clone https://github.com/Parthsharma91/IPL-ProScore.git
cd IPL-ProScore
```

---

## 🐍 Step 2: Create and Activate Virtual Environment

### ▶ Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### ▶ Mac/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 📦 Step 3: Install Required Packages

### 🛠 Make sure `setuptools`, `wheel`, and `build` are up to date:

```bash
pip install --upgrade pip setuptools wheel build
```

### 📦 Install the actual project dependencies:

```bash
pip install -r requirements.txt
```

> ⚠ If you face errors with `numpy`, open `requirements.txt` and replace:
> ```
> numpy==1.21.2
> ```
> with:
> ```
> numpy>=1.24
> ```

Then run the install command again.

---

## 🚀 Step 4: Run the App

```bash
python app.py
```

If needed, change the port in `app.py`:

```python
# Change this line:
app.run()

# To:
app.run(port=8000)
```

---

## 🌐 Step 5: Open in Browser

Once running, visit:

```
http://localhost:5000
```

or (if using a custom port):

```
http://localhost:8000
```

---

## 💡 Optional: Test Flask is Working

Create a `test_app.py` file and paste:

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return 'Flask is working!'

if __name__ == '__main__':
    app.run(debug=True)
```

Run it:

```bash
python test_app.py
```

Go to [http://localhost:5000](http://localhost:5000)

---

## 🧹 To Deactivate the Environment

```bash
deactivate
```

---

## 📫 Need Help?

Feel free to raise an issue on the [GitHub repo](https://github.com/Parthsharma91/IPL-ProScore/issues) or contact the maintainer.

---
