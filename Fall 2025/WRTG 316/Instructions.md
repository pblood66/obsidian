# 📘 CS 110 — Python Development Environment Setup  
*A beginner-friendly guide to getting your tools ready for programming.*

---

## 🌟 Introduction

Welcome to **CS 110**! In this class, you'll begin your journey into programming using **Python**, one of the world’s most widely used languages.

Before writing your first program, you’ll need to set up your computer with:

- **Python** (the programming language)
- **Visual Studio Code (VS Code)** (your editor)
- **The terminal** (your command-line workspace)
- **Virtual environments** (project-specific “bubbles” for Python)
- **Dependencies** (extra tools Python needs)

Each section below will walk you through installation, setup, and basic usage.  
Don’t worry if everything feels new—every programmer starts here!

---

# 🐍 Installing Python

### 1. Download Python  
Visit the official download page:  
https://www.python.org/downloads

Choose the installer that matches your operating system.

### 2. Download the latest version  
![placeholder](path/to/python-download.jpg)

### 3. Open the installer  
Follow the instructions based on your OS:

---

### **Windows**
📌 **IMPORTANT:** Check the box: **“Add Python to PATH.”**

Then choose **Install Now**.

![placeholder](path/to/windows-python-install.jpg)

---

### **MacOS**
Just open the installer and walk through the prompts—no extra steps needed.  
![placeholder](path/to/macos-python-install.jpg)

---

### 4. Verify the Installation

#### **Windows**
1. Open **Windows PowerShell**
2. Run:
   ```bash
   python --version
   ```
3. You should see something like:  
   ![placeholder](path/to/python-version-windows.jpg)

---

#### **MacOS**
1. Open **Terminal** (via Spotlight search)
2. Run:
   ```bash
   python3 --version
   ```
3. You should see something like:  
   ![placeholder](path/to/python-version-macos.jpg)

---

# 💻 Installing Visual Studio Code (VS Code)

### 1. Download VS Code  
https://code.visualstudio.com/download

Choose the installer that matches your OS.  
![placeholder](path/to/vscode-download.jpg)

---

### **Windows Installation**
1. Accept the license agreement  
2. Accept or change the destination folder  
3. Check these boxes:
   - **Add ‘Open with Code’ action**
   - **Add to PATH**

![placeholder](path/to/vscode-windows-options.jpg)

Click **Install**.

---

### **MacOS Installation**
Just open the installer—VS Code will set itself up automatically.  
![placeholder](path/to/vscode-macos.jpg)

---

### 2. Install the Python Extension
1. Open VS Code  
2. Go to the **Extensions** tab (left sidebar)  
3. Search for **Python**  
4. Install the official extension by Microsoft  
![placeholder](path/to/vscode-python-extension.jpg)

---

# 🖥️ Navigating the Terminal

You can open a terminal in VS Code:

- **Windows/Linux:** `CTRL + \``
- **MacOS:** `CMD + \``  
Or go to: **Terminal > New Terminal**

You can also open your system terminal:

- **Windows:** Search for *PowerShell*  
- **MacOS:** Search for *Terminal*

---

## 📂 Common Terminal Commands

| Command | Description |
|--------|-------------|
| `pwd` | Print working directory (current folder path) |
| `ls` | List files/folders in directory |
| `cd ..` | Move to parent directory |
| `cd path/to/folder` | Move to specific folder |
| `cd ~` | Go to home directory |
| `code folder` | Open folder/file in VS Code |
| `python file.py` | Run a Python file |
| `mkdir name` | Create a new folder |

---

# 📦 Creating a Virtual Environment

A **virtual environment** is a project-specific Python workspace.  
Every CS 110 project should use its own environment.

### 1. Open the Command Palette
- **Windows:** `CTRL + SHIFT + P`  
- **MacOS:** `CMD + SHIFT + P`

### 2. Search for:  
**Python: Create Environment**

### 3. Choose Environment Manager
Select: **venv**

### 4. Choose Interpreter  
Pick the **latest version of Python**.

### 5. Name the Environment  
We recommend leaving it as:  
```
.venv
```

### 6. Skip package installation  
(You’ll install packages manually later.)

### 7. You should see a `.venv` folder appear  
![placeholder](path/to/venv-folder.jpg)

---

## 🔌 Activating the Virtual Environment

### **Windows PowerShell**
```bash
.\.venv\Scripts\Activate.ps1
```

### **MacOS / Linux**
```bash
source ./.venv/bin/activate
```

You should now see:
```
(.venv)
```
on the left side of your terminal prompt.

🎉 Congratulations — your virtual environment is ready!

---

# 📥 Installing Dependencies & Libraries

Dependencies are extra tools that Python projects use.

For CS 110, you’ll need:

- `byu_pytest_utils`
- `numpy`
- `byubit`

### 1. Make sure your environment is active  
(You should see `(.venv)` in the terminal.)

### 2. Install packages:

```bash
pip install byu_pytest_utils
pip install numpy
pip install byubit
```

Each installation should look similar to:  
![placeholder](path/to/pip-install.jpg)

---

# ✅ You're Ready!

Your computer is now fully set up for CS 110:
- Python installed  
- VS Code configured  
- Terminal basics learned  
- Virtual environment created  
- Dependencies installed  

You’re ready to start coding! 🚀
