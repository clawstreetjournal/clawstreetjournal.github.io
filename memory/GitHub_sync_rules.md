# GitHub Sync Rules for clawstreetjournal

The local directory `/Users/finn/.openclaw/workspace/clawstreetjournal` must stay in sync with the GitHub repo:
- **Remote URL:** `https://github.com/clawstreetjournal/clawstreetjournal.github.io`
- **Git remote name:** `origin`
- **Primary branch:** `main`

### Rules:

1. **Use the existing clone, don't reclone**  
   Treat `/Users/finn/.openclaw/workspace/clawstreetjournal` as the only working copy. Do not run `git clone` into this folder if it already contains a `.git` directory.

2. **Always pull before making changes**  
   Before editing any files:
   ```bash
   cd /Users/finn/.openclaw/workspace/clawstreetjournal
   git status
   ```
   If there are no local changes:
   ```bash
   git pull --rebase origin main
   ```
   If there are local changes, either:
   - Commit them first (see below), or
   - Stash them:
   ```bash
   git stash
   git pull --rebase origin main
   git stash pop
   ```

3. **Make edits, then commit and push**  
   After you modify files (markdown, HTML, config as instructed):
   ```bash
   cd /Users/finn/.openclaw/workspace/clawstreetjournal
   git status
   git add -A
   git diff --cached
   ```
   If the staged diff looks correct, commit:
   ```bash
   git commit -m "clawstreetjournal: <short description of change>"
   git push origin main
   ```
   If `git push` fails because the remote has new commits:
   ```bash
   git pull --rebase origin main
   git push origin main
   ```

4. **Handle merge/rebase conflicts carefully**  
   If `git pull --rebase` reports conflicts:
   - Open each conflicted file, resolve conflicts conservatively (preserve existing content unless the user explicitly requested replacement). Then:
   ```bash
   git add -A
   git rebase --continue
   git push origin main
   ```
   - Never "solve" conflicts by deleting large sections of content unless explicitly instructed.

5. **Operate only in this directory**  
   Run all git commands from `/Users/finn/.openclaw/workspace/clawstreetjournal`. Do not create or use additional independent clones of `clawstreetjournal.github.io` elsewhere on disk.

6. **Respect Jekyll/GitHub Pages constraints**  
   - The repository `clawstreetjournal/clawstreetjournal.github.io` is a GitHub Pages Jekyll site. Do not modify `Gemfile`, `Gemfile.lock`, or `.github/workflows` unless explicitly asked.
   - Only make targeted changes to `_config.yml` when requested; do not add unsupported plugins.

7. **After pushing changes** that affect the website, check the GitHub Pages build status for this repo; if there is a build error, read the error message, fix that specific file, and push again.