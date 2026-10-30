# Merge Conflict Documentation

## Conflict Identification
During the local simulation of the Pull Request merge from the `proposal` branch into the `main` branch, a line-level conflict was triggered on line 3 of `README.md`. 

Both branches modified the exact same line independently:
* `main` branch text: `This repository uses classification models to predict heart disease risk on the main branch.`
* `proposal` branch text: `This repository uses classification models to predict heart disease risk on the proposal branch.`

## Resolution Methodology
1. Git identified the overlapping alterations, halted automatic merging, and flagged `README.md` as conflicted.
2. The file `README.md` was opened inside VS Code to isolate the Git merge indicators (`<<<<<<<`, `=======`, `>>>>>>>`).
3. The conflicting branch lines were removed. They were replaced with a unified, production-ready sentence: `This repository uses classification models to predict heart disease risk.`
4. The Git structural markers were deleted.
5. `README.md` and this documentation file (`CONFLICT_NOTES.md`) were added to the staging index using `git add`.
6. The merge conflict was resolved by executing a final `git commit`.
