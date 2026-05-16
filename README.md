# oil-supply-demand-balances

Personal project for retrieving oil market data from the U.S. EIA, cleaning/transformation, and computing supply-demand balances.

## Step-by-step: pull this GitHub repo to your local machine and open it in VS Code

### 1) Copy your repository URL from GitHub
1. Open your GitHub repository page.
2. Click **Code**.
3. Copy either:
   - **HTTPS** URL (easier to start), or
   - **SSH** URL (best if you already set up SSH keys).

Example:
- HTTPS: `https://github.com/<your-username>/oil-supply-demand-balances.git`
- SSH: `git@github.com:<your-username>/oil-supply-demand-balances.git`

### 2) Open Terminal on your computer
- **Windows**: PowerShell or Git Bash
- **Mac**: Terminal
- **Linux**: Terminal

### 3) Move to the folder where you want the project
```bash
cd path/to/your/projects
```

### 4) Clone the repository
```bash
git clone <repo-url>
```
Example:
```bash
git clone https://github.com/<your-username>/oil-supply-demand-balances.git
```

### 5) Enter the project folder
```bash
cd oil-supply-demand-balances
```

### 6) Open in VS Code
If `code` command is installed:
```bash
code .
```
If not installed:
- Open VS Code manually.
- Click **File → Open Folder...**
- Select `oil-supply-demand-balances`.

### 7) Verify Git is connected
Run:
```bash
git remote -v
```
You should see `origin` pointing to your GitHub repo.

---

## Daily workflow in VS Code (basic)

### Pull latest changes before work
```bash
git pull origin main
```

### Create a new feature branch
```bash
git checkout -b feat/eia-data-ingestion
```

### After editing files, commit and push
```bash
git add .
git commit -m "Add initial EIA ingestion scaffold"
git push -u origin feat/eia-data-ingestion
```

Then open a Pull Request on GitHub.

---

## Suggested first project structure

```text
oil-supply-demand-balances/
  data/
    raw/
    processed/
  notebooks/
  src/
    ingest/
    transform/
    balances/
  tests/
  README.md
  requirements.txt
```

---

## Next phase (oil balances scope)
1. Retrieve EIA oil-related series/data tables.
2. Normalize units, dates, and product naming.
3. Clean missing/duplicate observations.
4. Build transformed datasets by product and region.
5. Compute balances (e.g., supply - demand, stock changes).
6. Export tables/charts for reporting.

