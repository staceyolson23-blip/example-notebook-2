# 🔵 04a-activate-and-run-python-script.md

How to run a Python file (`.py`) in VS Code. 
For Jupyter notebooks (.ipynb), you don’t need these steps.

## Before Starting

- Open your project repository folder in VS Code. 
- Open a terminal. 
- If .venv is not active, activate the virtual environment (.venv).
- If external dependencies have not been installed, install them. 


## Task 1. Select VS Code Interpreter

VS Code needs our populated .venv to interpret our files correctly.

To set the VS Code Interpreter:

1. Open the Command Palette: Press Ctrl+Shift+P (Windows/Linux) or Cmd+Shift+P (Mac).
2. Search for "Python: Select Interpreter":
3. Type **Python: Select Interpreter** in the Command Palette search bar and select it from the dropdown.
4. Choose an Interpreter - A list of available Python environments will appear. Look for the recommended local .venv option.
5. Check the Python version shown in the lower-left status bar.


### Making Changes / Saving

Now we can get help from the VS Code editor while working on the Python code files. 

After making changes, run the file to verify following the steps below.
Save your files periodically to avoid losing progress - or ensure VS Code  **File / Autosave** option is on. 


## Windows Task 2: Activate and Execute

1. Ensure .venv is active. If active, you don't need to rerun the activate command.
2. Run the file. 

IMPORTANT: Change the name of the file to your actual file. 
The file must exist in the root project folder for the execute command to work. 

Run the following commands from the project root directory. 
The commands work in PowerShell.

```powershell
.\.venv\Scripts\activate
py myfile.py
```


## Mac/Linux Task 2: Activate/Execute

1. Ensure .venv is active. If active, you don't need to rerun the activate command.
2. Run the file.

IMPORTANT: Change the name of the file to your actual file. 
The file must exist in the root project folder for the execute command to work. 

Run the following commands from the project root directory. 
The commands work in zsh, bash, and more.

```powershell
source .venv/bin/activate
python3 demo-script.py
```


## AS-NEEDED: Add New External Dependencies

As you work, you may identify additional packages you want to use in your project. 
Add each package to requirements.txt and re-run the install dependencies process first. 

## Experience

- Understand why the virtual environment must be activated first. 
- Understand when adding a new external dependency, we must first add it to requirements.txt and re-run the install command. 
- Record your process and steps in your project README.md. 

---

[🔵 Continue with Part 3: Repeatable Workflow](REPEATABLE-WORKFLOW.md)
