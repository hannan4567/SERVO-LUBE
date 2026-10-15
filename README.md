# SERVO Dealer Hub

Static website. `index.html` is the whole site (no CSS/JS folders needed).
Data in `data/*.json` is auto-generated from `update-here/RATE_CHART.xlsx` by GitHub Actions.

## Deploy (new repo)
1. Create a new PRIVATE GitHub repo and upload ALL files of this folder (including hidden `.github`). Use GitHub Desktop.
2. GitHub: Settings -> Actions -> General -> Workflow permissions -> **Read and write**.
3. Vercel: Add New Project -> import repo -> Framework "Other" -> no build command, no output directory -> Deploy.

## Update rates
Upload new Excel into `update-here/` (replace RATE_CHART.xlsx). Wait ~2 minutes. Check Actions tab for a green tick.

## Announcements
Edit `data/announcements.json`. Set `"active": true` to show, `false` to hide.
