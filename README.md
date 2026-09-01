# Deadline Board

A single-page countdown board — add tasks with a deadline, and each one shows
days / hours / minutes remaining on a split-flap "departures" style display.
Data is saved in your browser (localStorage), so it persists between visits
on the same device/browser.

## Put it on your GitHub account (GitHub Pages)

I don't have write access to your GitHub account, so here's the quick manual
path — takes about 2 minutes:

1. Go to https://github.com/new and create a new repository (e.g. `deadline-board`). Public repo, no need to add a README/gitignore.
2. On the repo page, click **Add file → Upload files**, and upload `index.html` from this folder.
3. Commit the upload (straight to the `main` branch is fine).
4. Go to the repo's **Settings → Pages**.
5. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
6. Wait ~1 minute, then your site will be live at:
   `https://<your-username>.github.io/deadline-board/`

### If you'd rather use git from your terminal
```bash
git init
git add index.html
git commit -m "Add deadline board"
git branch -M main
git remote add origin https://github.com/<your-username>/deadline-board.git
git push -u origin main
```
Then do steps 4–6 above.

## Notes
- Tasks are stored per-browser (localStorage) — they won't sync across
  different devices or browsers automatically, since this is a static site
  with no backend.
- If you want it to say "Deadline Board" instead of "Departures", or want a
  different visual style, just ask — happy to adjust.
