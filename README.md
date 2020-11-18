# Jupytext Tutorial

Using Jupyter Notebooks is convenient but version control is a mess. This repository shows a brief example of [Jupytext](https://github.com/mwouts/jupytext). 

    pip install jupytext

Scripts and Notebooks are synchronized but notebooks are ignored (see `.gitignore`).

    .
    ├── .gitignore
    ├── jupytext.toml
    ├── notebooks           # contains notebooks (.ipynb)
    │   ├── .gitkeep
    │   └── test.ipynb
    ├── README.md
    └── scripts             # contains scripts (.py)
        └── test.py

If the repository has just been cloned, the corresponding notebooks can be created by

    jupytext --sync scripts/*.py
