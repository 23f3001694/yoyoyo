# CI Matrix Demo (55db92a)


This repo demonstrates a GitHub Actions **matrix build** across OS and Node versions, with parallel jobs and artifact upload.


- Matrix: `os = [ubuntu-latest, macos-latest, windows-latest]`, `node = [14, 16, 18]` (9 variants run in parallel)
- Each job writes a JSON build artifact and uploads it as `build-55db92a-<os>-v<node>`
- Includes the validation step identifier: `matrix-55db92a`


## My email
23f3001694@ds.study.iitm.ac.in


## How to run
1. Commit and push to `main` (or trigger manually with **Run workflow**).
2. Check **Actions → Matrix CI (55db92a)** for 9 successful matrix jobs.
3. Verify **Artifacts** show at least 3 entries prefixed `build-55db92a-` (there will be 9).
