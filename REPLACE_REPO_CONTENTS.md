# Replacing the Existing `Cosmology` Repository Contents

This folder is prepared as a clean replacement for the old repository contents.

## Recommended Workflow

1. Clone the existing repository if needed:

```bash
git clone <your-Cosmology-repo-url>
cd Cosmology
```

2. Remove the old tracked files from the working tree while keeping `.git`:

```bash
find . -mindepth 1 -maxdepth 1 ! -name .git -exec rm -rf {} +
```

3. Copy the prepared replacement contents from `github_upload` into the repository root:

```bash
cp -R /Users/waerbeke/Documents/RESEARCH/codexAI/cosmology/github_upload/. .
```

4. Review the result:

```bash
ls -la
git status
```

5. Commit and push:

```bash
git add -A
git commit -m "Replace old recombination notebook with documented teaching version"
git push
```

## What This Upload Contains

- the cleaned notebook `recombination.ipynb`
- a new `README.md`
- a minimal `requirements.txt`
- standard ignore rules in `.gitignore`

## Caution

Step 2 completely removes the old repository contents from the working tree. Make sure you do this in a clean clone or after confirming you no longer need the previous files.
