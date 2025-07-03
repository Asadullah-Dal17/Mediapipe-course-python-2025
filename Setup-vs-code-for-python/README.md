# 🛠️ Setting Up Your MediaPipe Python Development Environment

A quick and reliable guide for both **Linux** and **Windows** users to get started with MediaPipe and OpenCV in VS Code.

---

## 1️⃣ Install Python

### Linux 🐧
```bash
python3 --version  # Check if installed
sudo apt update
sudo apt install python3 python3-pip
```

### Windows 🪟
1. Download from [python.org](https://www.python.org/downloads/)
2. Run the installer (**check "Add Python to PATH"**)
3. Verify installation:
   ```cmd
   python --version
   ```

---

## 2️⃣ Create a Virtual Environment

### Linux 🐧
```bash
sudo apt install python3-venv  # If not already installed
python3 -m venv mediapipe_env
source mediapipe_env/bin/activate
```

### Windows 🪟
```cmd
python -m venv mediapipe_env
mediapipe_env\Scripts\activate
```

> **Tip:** Always activate your virtual environment before working on the project!

---

## 3️⃣ Install Required Packages

```bash
pip install --upgrade pip
pip install mediapipe opencv-python matplotlib numpy
```

- **For GPU acceleration:**
  ```bash
  pip install mediapipe-gpu
  ```
- **Linux webcam support:**
  ```bash
  sudo apt install v4l-utils
  ```
- **Deactivate environment:**
  ```bash
  deactivate
  ```

---

## 4️⃣ VS Code Setup

1. **Install VS Code:** [Download here](https://code.visualstudio.com/)
2. **Recommended Extensions:**
    - Python (Microsoft)
    - Pylance
    - IntelliCode
    - Path Intellisense
    - Jupyter (optional)
    - Black Formatter (Python code formatter)
    - Code Spell Checker
    - Emojisense
3. **Select Interpreter:**
   - Press `Ctrl+Shift+P` → type `Python: Select Interpreter` → choose your virtual environment.

### Install Extensions via Terminal

#### Linux 🐧
```bash
code --install-extension ms-python.python \
     --install-extension ms-python.vscode-pylance \
     --install-extension christian-kohler.path-intellisense \
     --install-extension VisualStudioExptTeam.vscodeintellicode \
     --install-extension ms-python.black-formatter \
     --install-extension bierner.emojisense \
     --install-extension streetsidesoftware.code-spell-checker
```

#### Windows 🪟
```powershell
code --install-extension ms-python.python `
     --install-extension ms-python.vscode-pylance `
     --install-extension christian-kohler.path-intellisense `
     --install-extension VisualStudioExptTeam.vscodeintellicode `
     --install-extension ms-python.black-formatter `
     --install-extension bierner.emojisense `
     --install-extension streetsidesoftware.code-spell-checker
```

---

## 📝 Additional Notes

- Keep your dependencies updated for best performance.
- Use a `.gitignore` to avoid committing your `mediapipe_env` folder.
- For troubleshooting, check the [MediaPipe documentation](https://google.github.io/mediapipe/) or [OpenCV documentation](https://docs.opencv.org/).

---

Happy coding! 🚀
