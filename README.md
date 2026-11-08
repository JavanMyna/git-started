# Git & GitHub Pages Playground

A single-file learning page for beginners, built for the "Gitting Over It" workshop (GDG on Campus, USM). It has a pretend terminal for practising Git commands safely, a short "go live" checklist for GitHub Pages, a few fixes for common errors and a small cheat sheet.

No build step, no dependencies. Everything (HTML, CSS, JS) lives in `index.html`.

**Dont confuse this website link with the one you will create later!**
>   **Live page:** https://javanmyna.github.io/git-started/

## Use it in the workshop

1. **Fork** this repo (Fork button, top right).
2. **Clone** your fork and open the folder:
   ```
   git clone <your-fork-url>
   cd git-started
   ```
3. Edit `index.html`, then save your work:
   ```
   git add .
   git commit -m "my first change"
   git push
   ```
4. **Turn on Pages:** your fork > Settings > Pages > Deploy from a branch > `main` / (root) > Save.
5. Wait about a minute, then open `https://YOUR-USERNAME.github.io/git-started/`.

### Put your own HTML file online

Copy any HTML file (for example a CCA102 tutorial file) into the folder, then add, commit and push it. It appears at:

`https://YOUR-USERNAME.github.io/git-started/yourfile.html`

- Use a filename with no spaces. Names are case-sensitive, so `Tutorial3.html` and `tutorial3.html` are different.
- Copy any images or CSS files the page uses too.
- GitHub Pages sites are public. Only publish practice work.

## What's inside the page

| Section | What it does |
|---|---|
| **Practice** | A simulated terminal with six missions: init, add, commit, branch, merge, push. |
| **Go live** | A six-step checklist (progress saved in the browser) and a URL builder. |
| **The loop** | edit, add, commit, push in one line. |
| **Stuck?** | Fixes for the most common beginner errors. |
| **Cheat sheet** | Six commands. Tap one to copy it. |

## Limits to know about

- It is a simulation, not real Git. It never touches your files.
- No merge conflicts, remotes, tags or rebasing.
- `cd` does nothing; you always stay in `my-site`.
- Only the checklist progress is saved (in `localStorage`). The terminal resets when you reload.

## Credits

Visual style follows the Google Developer Groups (GDG) presentation theme.
