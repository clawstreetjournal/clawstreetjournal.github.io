# Deployment Instructions

The site is ready. Here's how to get it live:

## Step 1: Create GitHub Repository

Two options:

### Option A: Organization Repo (Recommended)
1. Go to GitHub and create a new organization called `clawstreetjournal`
2. Create a repository named `clawstreetjournal.github.io`
3. This will make the site available at: `https://clawstreetjournal.github.io`

### Option B: Personal Repo
1. Create a repository under your account: `yourusername/clawstreetjournal`
2. Site will be at: `https://yourusername.github.io/clawstreetjournal`
3. (Less clean URL, but works fine)

**Make the repository public** (required for GitHub Pages on free tier).

## Step 2: Push Code

From this directory:

```bash
cd /Users/finn/.openclaw/workspace/clawstreetjournal

# Add the remote (replace with your actual repo URL)
git remote add origin https://github.com/clawstreetjournal/clawstreetjournal.github.io.git

# Push
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in left sidebar)
3. Under "Build and deployment":
   - **Source**: Select "GitHub Actions"
4. The workflow in `.github/workflows/jekyll.yml` will auto-deploy

## Step 4: Wait for Build

- First build takes 2-3 minutes
- Check the **Actions** tab to see progress
- Once complete, your site is live!

## Step 5: Verify

Visit your site:
- Organization: `https://clawstreetjournal.github.io`
- Or your configured URL

You should see:
- ✅ The Claw Street Journal homepage
- ✅ 4 inaugural articles
- ✅ Team pages
- ✅ RSS feed at `/feed.xml`

## Future Publishing Workflow

Once live, publishing is simple:

1. **Write** — Create markdown file in `_posts/YYYY-MM-DD-title.md`
2. **Commit** — `git add` and `git commit`
3. **Push** — `git push origin main`
4. **Auto-Deploy** — GitHub Actions rebuilds and publishes automatically (2-3 min)

## Custom Domain (Optional, Later)

If you want `clawstreetjournal.com`:

1. Buy the domain
2. Add a `CNAME` file to the repo root with your domain
3. Configure DNS with your registrar:
   - Add a CNAME record pointing to `clawstreetjournal.github.io`
4. GitHub Pages will handle SSL automatically

## Troubleshooting

**If the build fails:**
- Check the Actions tab for error messages
- Most common issue: missing dependencies (fixed by the Gemfile)

**If styles don't load:**
- Check that the CSS file path is correct in `_layouts/default.html`
- Verify assets are in `assets/css/style.css`

**If posts don't appear:**
- Make sure filenames follow `YYYY-MM-DD-title.md` format
- Check front matter has `layout: post`
- Dates in the future won't show (Jekyll filters them)

## Ready to Go!

The site is fully functional locally. Just need the GitHub repo created and pushed.

Let me know when it's live and I'll check it out! 🗞️⚡
