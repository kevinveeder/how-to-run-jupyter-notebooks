# how-to-run-jupyter-notebooks
This is a simple walkthrough of how to run jupyter notebooks if you've never installed it before. 

### Requirements for this walkthrough:
- This tutorial uses Anaconda for most of the steps. If you don't have anaconda installed, there are equivalent terminal comnmands you can run but they arent listed here.
- To download the anaconda installer:  https://www.anaconda.com/products/distribution 
---
## 1. Clone (or download) repo
First, clone the repo to your local machine (run these in terminal)
- *__Note:__* replace `NAME-OF-MY-REPO` with the name of the repo that you want to clone
```
git clone https://github.com/kevinveeder/NAME-OF-MY-REPO.git
cd NAME-OF-MY-REPO
```

---
## 2. Create virtual environment

Run these in anaconda prompt
- This will set up a virtual environment to avoid conflicting dependencies (optional, but recommended):
```
conda create -n clean_env python=3.11

conda activate clean_env
```
---
## 3. Download and run jupyter notebooks (if not installed)
Run these in anaconda prompt
- This will download jupyter notebooks and some of my common libraries:
``` 
conda install notebook jupyterlab numpy pandas matplotlib scikit-learn

jupyter notebook
```
---
## 4. Navigate to .ipynb file -> Run
- A browser window will open with Jupyter Notebook. Navigate to the .ipynb file that you downloaded in step 1 and run cells
