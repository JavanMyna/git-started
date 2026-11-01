# Git & GitHub Pages Playground

A single-file learning page for beginners, built for a GDG workshop. It has a pretend terminal where you can practise Git commands safely, plus short explanations, a "go live" checklist, a troubleshooting section and a cheat sheet.

No build step, no dependencies. Everything (HTML, CSS, JS) lives in `index.html`.

## What's inside

| Section | What it does |
|---|---|
| **Practice** | A simulated terminal with six missions: init, add, commit, branch, merge, push. Tap a chip or type the commands. |
| **Learn** | Why Git, Git vs GitHub, branches, and the add → commit → push loop. |
| **Go live** | A five-step GitHub Pages checklist (progress is saved in the browser) and a URL builder for `username.github.io/repo`. |
| **Stuck?** | Fixes for common beginner errors, such as not a git repository, authentication failed, nothing to commit and Pages 404. |
| **Cheat sheet** | Twelve essential commands. Tap one to copy it. |
| **Say hi** | A short card for your contact details. |

## Run it

Open `git-playground.html` in any modern browser. That's it.

The fonts (Outfit and Roboto Mono) load from Google Fonts. If you're offline, the page falls back to system fonts and still works.

## Host it on GitHub Pages

```bash
git init
git add .
git commit -m "add playground"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

Then on GitHub: **Settings → Pages → Deploy from a branch → `main` / (root) → Save**.

Your page will be live in about a minute at:

- `https://YOUR-USERNAME.github.io/YOUR-REPO/git-playground.html`, or
- `https://YOUR-USERNAME.github.io/YOUR-REPO/` if you rename the file to `index.html`.

## Make it yours

- **Contact card:** search for `@your-handle` and replace both spots in the "Let's study together" section (`#hi`). Edit the intro text there too.
- **Checklist:** edit the `<label>` items inside `#steps`.
- **Troubleshooting:** add or remove `<details>` blocks inside `#stuck`.
- **Cheat sheet:** edit the `CH` array near the bottom of the script.
- **Quick-run chips:** edit the array of command strings just above the `reset` button handler.
- **Colours:** change the CSS variables at the top of the `<style>` block. They follow the GDG palette and switch automatically for dark mode.

## Commands the practice terminal understands

| Command | Notes |
|---|---|
| `echo "text" > file`, `echo "text" >> file` | Creates or changes a file |
| `touch file`, `ls`, `pwd`, `clear`, `help` | Basics |
| `git --version` | Prints a fake version number |
| `git init` | Starts a repo |
| `git status` | Shows staged, modified and untracked files |
| `git add .` / `git add file` | Stages changes |
| `git commit -m "msg"` | Also accepts `-am` |
| `git log`, `git log --oneline` | Shows history |
| `git branch`, `git branch name` | Lists or creates branches |
| `git switch name`, `git switch -c name` | `checkout` and `-b` also work |
| `git merge name` | Fast-forward, or a simple merge commit |
| `git push` | Simulated, with a hint about turning on Pages |
| `git pull` | Always says "Already up to date" |

Use the up and down arrow keys to scroll through your command history. Press **Start over** to reset the missions and the repo.

## Limits to know about

- It is a simulation, not real Git. It never touches your files.
- There are no merge conflicts, remotes, tags or rebasing.
- `cd` does nothing; you always stay in `my-site`.
- Only the checklist progress is saved (in `localStorage`). The terminal state resets when you reload.

## Credits

Visual style follows the Google Developer Groups (GDG) presentation theme: Google blue, red, yellow and green on an off-white background.

<.