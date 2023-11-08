Repo to show ruff formatter not working for notebooks in pre-commit

Create a notebook that needs formatting. It will contain a cell that looks like

`_l = [1, 2, 3,]`

Run it in a GitHub Action to show it passes pre-commit whereas it should fail
