# webpro-w9

Week 9 homework for Web Programming (K0126002, Gachon University) by Sukhrob.
It covers the Git exercises E1 to E3 from the Week 9 study guide.

Live page: https://msukhrob.github.io/webpro-w9/

## Commands used and what they did

### E1 - first repository and first commit
| Command | What it does |
|---|---|
| `git clone https://github.com/MSukhrob/webpro-w9.git` | Downloads the empty GitHub repository (it already has `origin` set, so it replaces `git init` + `git remote add`) |
| `git checkout -b main` | Creates and switches to the `main` branch |
| `git status` | Shows that `index.html` is untracked |
| `git add index.html` | Stages the file |
| `git commit -m "Initial commit: add index.html"` | Saves the first snapshot |
| `git log --oneline` | Shows the commit history |

### E2 - branch and merge
| Command | What it does |
|---|---|
| `git checkout -b feature-style` | Creates a feature branch and switches to it |
| `git add style.css index.html` | Stages the new stylesheet and the `<link>` in the HTML |
| `git commit -m "Add basic stylesheet"` | Commits the change on the feature branch |
| `git checkout main` | Goes back to `main` (`style.css` disappears from the folder) |
| `git merge --no-ff feature-style -m "Merge feature-style into main"` | Merges the branch and keeps a merge commit, so the branch is visible in the history |
| `git log --oneline --graph` | Shows the branch and merge as a graph |

### E3 - push to GitHub
| Command | What it does |
|---|---|
| `git push -u origin main` | Uploads all commits to GitHub and links local `main` with `origin/main` |

### Later
| Command | What it does |
|---|---|
| `git add README.md` and `git commit -m "Add README with git commands used"` | Adds this documentation |
| `git push` | Uploads the new commit |

## What was done
1. Created the public repository `webpro-w9` on GitHub without a README.
2. Added `index.html` with my name and the date, and made the first commit.
3. Created the branch `feature-style`, added `style.css`, committed, and merged it into `main`.
4. Pushed everything to GitHub.
5. Enabled GitHub Pages (Settings, Pages, Deploy from branch, `main`, `/(root)`).
