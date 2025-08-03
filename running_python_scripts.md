# Running My Python Scripts (Windows)

Quick setup guide to get any of my Python projects up and running on your Windows machine.

## Prerequisites

- Windows operating system
- Python 3.7 or higher installed on your system
- Git installed (for cloning repositories)
- Internet connection (for installing packages)

## Setup Instructions

Follow these steps in order:

### 1. Clone the Repository
```bash
git clone <repo_name>
cd <project_directory>
```

### 2. Create Virtual Environment
```bash
python -m venv new_env
```

### 3. Activate Virtual Environment
```bash
new_env/Scripts/activate
```
*Note: You should see `(new_env)` appear at the beginning of your command prompt*

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```

### 5. Run the Script
```bash
python <python_script>
```

## Example Workflow

```bash
git clone https://github.com/username/my-awesome-project
cd my-awesome-project
python -m venv new_env
new_env/Scripts/activate
pip install -r requirements.txt
python main.py
```

## Troubleshooting

- **If you get a "python not recognized" error:** Make sure Python is added to your system PATH
- **If activation doesn't work:** Try using `new_env\Scripts\activate.bat` instead
- **If packages fail to install:** Make sure you're in the activated virtual environment

## When You're Done

To deactivate the virtual environment:
```bash
deactivate
```

---

*Replace `<repo_name>`, `<project_directory>`, and `<python_script>` with the actual values for each specific project.*
