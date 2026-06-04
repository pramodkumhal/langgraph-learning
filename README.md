
LangGraph Learning Notebooks
============================

This repository contains learning notebooks for LangGraph — a personal learning workspace where you explore LangGraph concepts, build small agent demos, and document experiments.

Overview
--------

- This is a collection of notebooks and examples for learning LangGraph.
- Examples include a basic chatbot demo and a human-in-the-loop assistance notebook to illustrate agent workflows.

Project structure
-----------------

Repository tree (top-level)

```text
.
├─ .git/
├─ .venv/               # local virtual environment (ignored)
├─ .env                 # local credentials (DO NOT commit)
├─ main.py
├─ pyproject.toml
├─ requirements.txt
├─ uv.lock
├─ 1-BasicChatbot/
│  └─ Chatbot.ipynb
├─ 2-HumanAssistance/
│  └─ humanintheloop.ipynb
└─ README.md
```

Notes:
- `.env` should be kept local and listed in `.gitignore`.
- Clear notebook outputs before committing to keep diffs small and avoid leaking data.
- Keep `uv.lock` for reproducible installs when using `uv`.

Dependencies and tooling
------------------------

- This workspace uses the `uv` package/tool for dependency management instead of relying solely on `pip`.
- Use your local `uv` workflow to install dependencies (example shown below). If you prefer `pip`, the `requirements.txt` file is provided for reference.

Getting started
---------------

1. Create and activate a virtual environment (recommended):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies with `uv` (if you use it):

```powershell
uv install
```

Or install using `pip` if you prefer:

```powershell
pip install -r requirements.txt
```

3. Run quick examples or open the notebooks in Jupyter Lab / Notebook:

```powershell
python main.py
```

Usage notes
-----------

- Open the notebooks to follow step-by-step experiments; run cells from top to bottom.
- Adapt `main.py` to point to your preferred Langgraph runtime or LLM backend when needed.

Contributing
------------

This is primarily a personal learning repository. Contributions or suggestions are welcome — open an issue or submit a pull request if you'd like to share improvements or additional notebooks.

License
-------

Add a `LICENSE` file if you wish to apply an open-source license (e.g., MIT).

