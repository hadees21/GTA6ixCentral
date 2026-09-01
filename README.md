# Task: Deploy GTA6ixCentral Hub site to GitHub Pages

## Context
Static single-file website for a GTA 6 fan tracker project. File exists
locally, repo is public — just needs to be committed, pushed, and Pages
enabled.

- Local repo path: /Users/hkhokhar/Documents/projects/GTA6ixCentral
- GitHub repo: https://github.com/hadees21/GTA6ixCentral (now PUBLIC)
- Remote "origin" is already set correctly to this repo.
- index.html exists in the local repo folder already — confirm with
  `ls` before assuming anything is missing.
- Local git identity should use my personal account, NOT my global
  work git config — do not use --global for user.name/user.email here.
  Check `git config user.email` (no --global) reflects my personal
  email before committing.
- Earlier issue: a cached GitHub credential for an unrelated account
  (hadees-chicago-bulls) without push access caused a 403 at one point.
  If that resurfaces, check Keychain Access (Mac) for cached
  github.com credentials before assuming anything else is wrong.

## What I need you to do
1. Run `git status` and `ls` to confirm current state — don't assume
   anything needs redoing without checking first.
2. If index.html isn't tracked/committed yet, `git add index.html` and
   commit with a clear message.
3. Push to origin/main. If it's rejected as non-fast-forward, explain
   what that means and run `git pull origin main --allow-unrelated-histories`
   before pushing again — don't force-push without telling me what
   would be lost.
4. Once pushed, walk me through enabling GitHub Pages in repo Settings
   → Pages → Source: Deploy from branch → main → /root → Save.
5. Confirm the final live URL once Pages is reachable
   (likely https://hadees21.github.io/GTA6ixCentral/).
6. Once live, briefly check that the page loads and isn't blank/broken
   (e.g. via curl or by telling me to open it in browser) — this file
   uses external Google Fonts links and inline JS for a countdown timer,
   quiz, and price tracker table, so confirm nothing looks obviously
   missing.

## Constraints
- Do not force-push without explicitly telling me what would be lost.
- Repo visibility is already public — no action needed there.