# 🧹 Hack a Lint
This repo is sample code of PyCon talk
```Hidden Hacks in Linters for Better & More Secure Code```

## Custom PyLint Checkers
* `redundant_class_chekcer.py` Warn if a class has no `__init__` function or it has no `self` assignment
* `http_client_checker.py` Verify that all http calls made in `http_client.py` class
* `golden_hammer_checker.py` Verify there is no long same `if` experssion

## VSCode integration
The `.vscode` folder include both VSCode config files
* `settings.json` config all chekcers to work with pylint
* `launch.json` contain debug config for all linters

The best way to make the script works is:
1. Use `virtualenvs` to create `venv` on workspace dir
2. Run `pip install -r requirements.txt` after activate env
3. Create `.env` file on workspace folder with right PYTHONPATH (following should contain `PYTHONPATH=.`)
