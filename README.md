# Beginner's Guide: Running Jupyter Notebooks

This guide will walk you through everything you need to clone repositories and run Jupyter notebooks, even if you've never used them before.

## What You'll Need

Before starting, make sure you have:
- **Git** - for cloning repositories
- **Python 3.8+** - for running Jupyter notebooks
- **Terminal/Command Prompt** - we'll use command line tools

## Step 1: Install Prerequisites

### Install Git (if not already installed)
- **Windows**: Download from [git-scm.com](https://git-scm.com/download/win)
- **Mac**: Install via Homebrew: `brew install git` or download from [git-scm.com](https://git-scm.com/download/mac)
- **Linux**: `sudo apt install git` (Ubuntu/Debian) or `sudo yum install git` (CentOS/RHEL)

### Install Python (if not already installed)
- Download from [python.org](https://www.python.org/downloads/)
- **Important**: During installation, check "Add Python to PATH"

### Verify installations
Open your terminal and run:
```bash
git --version
python --version
```
You should see version numbers for both.

## Step 2: Clone the Repository

Replace `NAME-OF-MY-REPO` with the actual repository name you want to clone:

```bash
git clone https://github.com/kevinveeder/NAME-OF-MY-REPO.git
cd NAME-OF-MY-REPO
```

## Step 3: Set Up Python Environment

Create a virtual environment to keep dependencies organized:

```bash
# Create virtual environment
python -m venv jupyter_env

# Activate it (choose the command for your system)
# Windows:
jupyter_env\Scripts\activate

# Mac/Linux:
source jupyter_env/bin/activate
```

**Note**: When the environment is active, you'll see `(jupyter_env)` at the beginning of your terminal prompt.

## Step 4: Install Jupyter and Common Libraries

With your virtual environment activated, install the necessary packages:

```bash
# Upgrade pip first
python -m pip install --upgrade pip

# Install Jupyter and common data science libraries
pip install jupyter numpy pandas matplotlib scikit-learn seaborn plotly
```

## Step 5: Start Jupyter Notebook

Launch Jupyter Notebook:

```bash
jupyter notebook
```

This will:
1. Start the Jupyter server
2. Automatically open your web browser
3. Display the Jupyter file browser

## Step 6: Open and Run Your Notebook

1. In the browser window that opened, navigate through the folders to find your `.ipynb` file
2. Click on the notebook file to open it
3. Run cells by:
   - Clicking a cell and pressing `Shift + Enter`
   - Or using the "Run" button in the toolbar
   - Or going to Cell → Run All to run everything

## Troubleshooting

### Common Issues and Solutions

**"Command not found" errors:**
- Make sure Python and Git are properly installed and added to your PATH
- Try `python3` instead of `python` on Mac/Linux

**Permission errors:**
- On Mac/Linux, you might need to use `python3 -m pip` instead of just `pip`
- Never use `sudo` with pip in a virtual environment

**Browser doesn't open automatically:**
- Look for a URL in the terminal output (usually `http://localhost:8888`)
- Copy and paste it into your browser manually

**Packages not found in notebook:**
- Make sure your virtual environment is activated when you run `jupyter notebook`
- If issues persist, install packages again with the environment activated

## Useful Commands

```bash
# Deactivate virtual environment when done
deactivate

# Reactivate environment later
# Windows:
jupyter_env\Scripts\activate
# Mac/Linux:
source jupyter_env/bin/activate

# Install additional packages (with environment activated)
pip install package_name

# List installed packages
pip list

# Stop Jupyter server
# Press Ctrl+C in the terminal where Jupyter is running
```

## What's Next?

Once you have Jupyter running:
- Cells with code can be edited and re-run
- Use `Shift + Enter` to run cells quickly
- Save your work with `Ctrl + S` (or `Cmd + S` on Mac)
- Create new cells with the "+" button or Insert menu

Happy coding! 🚀

---

**Need help?** If you run into issues, feel free to reach out (contact info on [readme](https://github.com/kevinveeder/kevinveeder)) or check the [Jupyter documentation](https://jupyter.org/documentation).
