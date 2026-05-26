# Gigachad — Static Site (local cache)

This repository contains a static, locally cached copy of the site branded as "Gigachad" for testing.

How to push this repo to GitHub (easy):

1. If you used `gh auth login --web` and completed auth, run:

```bash
git branch -M main
gh repo create saurabh30-bit/gigachad-site --public --source=. --remote=origin --push
```

2. If you prefer to create the repo in the browser, then run:

```bash
git branch -M main
git remote add origin https://github.com/saurabh30-bit/gigachad-site.git
git push -u origin main
```

If you ever use a PAT in a URL to push, immediately remove it from the remote after push and revoke the token in GitHub settings.

Deploy to Vercel (once the repo is on GitHub):

1. Visit https://vercel.com and import the repository `saurabh30-bit/gigachad-site` (connect GitHub if necessary).
2. For a static site choose the default `Framework Preset` → `Other` and set the output directory to `.` (site root). Then deploy.

Files added to help deploy:
- `vercel.json` — minimal configuration for a static deployment.

If you want, I can attempt the GitHub push and Vercel deploy for you — I only need you to complete one of the auth options we discussed (web `gh` auth or a PAT entered in your terminal). I cannot accept tokens pasted into chat.
