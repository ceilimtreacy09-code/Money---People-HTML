# Money & People — Operations Manual

A single-page, offline-first tracker for two self-taught skills: money
management and people/communication skills, plus a business track. Built
around an XP/leveling system, daily drills, a decision journal, and
reference material.

No backend, no build step, no dependencies — it's one self-contained
`index.html` file. All progress is saved locally in the browser via
`localStorage`.

## Deploy on GitHub Pages

1. Create a new repo (or use this one) and push these files to it.
2. In the repo on GitHub: **Settings → Pages**.
3. Under "Build and deployment", set **Source** to `Deploy from a branch`.
4. Pick the branch (usually `main`) and folder `/ (root)`, then **Save**.
5. GitHub will give you a URL like `https://<username>.github.io/<repo>/`
   within a minute or two — that's your live app.

### Quick way from the command line

```bash
git init
git add .
git commit -m "Money & People OS"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then turn on Pages as above.

## Notes

- Data is stored **per browser, per device** (`localStorage`) — it will not
  sync between your phone and laptop. Use the in-app **Data** tab to export
  a JSON backup and import it elsewhere.
- On mobile, open the deployed URL and use "Add to Home Screen" to make it
  launch like a standalone app.
- No API keys, no external services, nothing to configure — it just needs
  to be served as static files.
