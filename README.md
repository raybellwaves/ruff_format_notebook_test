Repo to show ruff formatter not working for notebooks in pre-commit

Create a notebook that needs formatting. It will contain a cell that looks like

`_l = [1, 2, 3,]`

Run it in a GitHub Action to show it passes pre-commit whereas it should fail.

You can see it works locally using ruff on the command line as:
```
git clone git@github.com:raybellwaves/ruff_format_notebook_test.git
cd ruff_format_notebook_test
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
ruff format . --check
```

You can see it doesn't work using pre-commit as:
```
pre-commit run --all-files ruff
```
