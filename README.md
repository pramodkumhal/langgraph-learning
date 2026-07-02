
LangGraph Learning Notebooks
============================

This repository is a personal learning workspace for LangGraph. It collects small notebook-based experiments covering chatbot flows, human-in-the-loop review, conditional routing, parallel workflows, iteration, and persistence.

Overview
--------

- Notebook-first examples for exploring LangGraph concepts.
- Lightweight Python entry point in `main.py` for quick smoke tests.
- Dependency lockfile included for reproducible installs with `uv`.

Project structure
-----------------

```text
.
├─ main.py
├─ pyproject.toml
├─ requirements.txt
├─ uv.lock
├─ 1-BasicChatbot/
│  └─ Chatbot.ipynb
├─ 2-HumanAssistance/
│  └─ humanintheloop.ipynb
├─ 3-Parallel_Workflow/
│  ├─ batsman_workflow.ipynb
│  └─ essay_workflow.ipynb
├─ 4-Conditional_Workflow/
│  ├─ quadratic_equation_workflow.ipynb
│  └─ review_reply_workflow.ipynb
├─ 5-Iterative_workflow/
│  └─ post_generator.ipynb
├─ 6-chatbot/
│  └─ baisc_chatbot.ipynb
└─ 7-Persistence/
	└─ persistence.ipynb
```

Setup
-----

Prerequisites:

- Python 3.14 or newer
- `uv` recommended for dependency management

Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install dependencies with `uv`:

```powershell
uv sync
```

If you prefer `pip`, use the requirements file:

```powershell
pip install -r requirements.txt
```

Usage
-----

- Open the notebooks in VS Code or Jupyter and run them from top to bottom.
- Run the Python entry point as a quick environment check:

```powershell
python main.py
```

Repository notes
----------------

- Keep `.env` local and out of version control.
- Clear notebook outputs before committing to keep diffs small.
- Keep `uv.lock` committed so installs stay reproducible.