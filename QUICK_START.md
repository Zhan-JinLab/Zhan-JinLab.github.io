# Quick Start Guide

## For the Impatient 🚀

### Deploy to GitHub Pages (5 minutes)

1. **Create GitHub organization** (recommended):
   - Go to GitHub → New organization
   - Name it (e.g., `zhanjin-lab`)

2. **Create repository**:
   - In your org: New repository
   - Name: `zhanjin-lab.github.io` (use your org name)
   - Public repository

3. **Push code**:
   ```bash
   cd zhanjin-lab-website
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-ORG/YOUR-ORG.github.io.git
   git push -u origin main
   ```

4. **Enable GitHub Pages**:
   - Repository Settings → Pages
   - Source: Branch `main`, folder `/` (root)
   - Save

5. **Done!** Visit `https://YOUR-ORG.github.io` in 1-2 minutes

---

## Test Locally First (Optional)

```bash
cd zhanjin-lab-website
bundle install
bundle exec jekyll serve
```

Open: http://localhost:4000

---

## Common Tasks

### Add a news post

1. Create: `_posts/2025-12-15-my-news.md`
2. Add content:
   ```markdown
   ---
   layout: post
   title: "My News Title"
   date: 2025-12-15
   ---
   
   News content here...
   ```
3. Commit and push

### Add publications

1. Edit: `_data/publications_jin.yml` or `_data/publications_zhan.yml`
2. Add under correct year:
   ```yaml
   - title: "Paper title"
     authors: "Authors list"
     journal: "Journal info"
     citations: 10
     doi: null
     topic: "CAR-T"
   ```
3. Commit and push

### Update team

1. Edit: `people.md`
2. Add/modify team member sections
3. Commit and push

---

## Getting Help

- Full documentation: see `README.md`
- Jekyll docs: https://jekyllrb.com/docs/
- Issues? Check Troubleshooting section in README

---

## Site URLs After Deployment

- **Organization account**: `https://zhanjin-lab.github.io`
- **Personal account**: `https://username.github.io/repo-name`

Update `_config.yml` if using a project repository (not org.github.io):
```yaml
baseurl: "/repo-name"
```

