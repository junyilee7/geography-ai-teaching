# Maintenance Notes

This file is for the repository maintainer.

## Regenerating the notebooks

The three notebooks are generated from a single script so they stay consistent:

```bash
python _build_notebooks.py
```

This rewrites the files under `notebooks/`.

## Test-running before committing

Optionally re-execute each notebook so the embedded plots match the latest code:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt jupyter nbconvert
for nb in notebooks/*.ipynb; do
  jupyter nbconvert --to notebook --execute "$nb" --output "$(basename "$nb")"
done
```

All three notebooks have been test-run end-to-end and complete without errors on a clean environment.

## Adding a new notebook

1. Add a new `make_notebook([...])` block in `_build_notebooks.py`.
2. Register its output filename in the `main()` function.
3. Add a row to the table in `README.md`.
4. Re-run `_build_notebooks.py` and test-execute.

## Publishing updates

```bash
git add .
git commit -m "Describe the update"
git push
```
