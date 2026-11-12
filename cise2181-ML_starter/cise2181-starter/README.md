# CISE2181 Machine Learning · Fall 2026 · Defect detection on MVTec AD

Starter repository for the Topic 10 transfer-learning lab and the midterm project.

## 1. Set up (Windows cmd, ST301 or your own PC)

```bat
D:
cd \cise2181
git clone https://github.com/YunTech-CISE2181/cise2181-starter.git
cd cise2181-starter
uv sync
uv run python -c "import torch; print(torch.__version__, torch.cuda.is_available())"
```

`uv sync` creates `.venv` and installs the exact versions in `uv.lock`.
Do not use `pip install`; add packages with `uv add <package>` so the lock file stays correct.

## 2. Data

MVTec AD is not in this repository. On ST301 it is at `D:\datasets\mvtec_ad`
(set `DATA_ROOT` in the notebook if it is elsewhere). On your own PC, download it
from mvtec.com and put it in `data\mvtec_ad`.

## 3. Run the lab

```bat
uv run jupyter lab
```

Open `notebooks/Topic10_Transfer_Learning_MVTecAD.ipynb` and run the cells in order.
Stop Jupyter with Ctrl+C in the cmd window.

## 4. Save your work

```bat
git status
git add notebooks
git commit -m "Run Topic 10 lab on tile and transistor"
git push
```

Clear notebook outputs (Kernel > Restart Kernel and Clear Outputs) before committing a notebook.

Reference: Git tutorial, https://git-scm.com/docs/gittutorial
