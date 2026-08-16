Downloads folder for AI-Assisted ICU Quality Review Workbench.

Software_System.zip is the separate runnable product deliverable. It is packaged from the current Software_System folder and excludes .git, .venv, __pycache__, logs, .env, data/software_system.db, and raw MIMIC source files.

To run after extraction:

Git Bash:
cd Software_System
python -m venv .venv
source .venv/Scripts/activate
pip install -r requirements.txt
./.venv/Scripts/python.exe app.py

PowerShell:
cd Software_System
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
.\.venv\Scripts\python.exe app.py

Open http://127.0.0.1:5000/ in a browser after the app starts.
