# Zhan/Jin Laboratory Website

A professional academic laboratory website built with Jekyll and GitHub Pages.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Local Development](#local-development)
- [GitHub Pages Deployment](#github-pages-deployment)
  - [Option 1: Organization Account (Recommended)](#option-1-organization-account-recommended)
  - [Option 2: Personal Account](#option-2-personal-account)
- [Content Management](#content-management)
  - [Adding Publications](#adding-publications)
  - [Creating News Posts](#creating-news-posts)
  - [Updating Team Members](#updating-team-members)
  - [Adding Photos](#adding-photos)
- [Customization](#customization)
- [Troubleshooting](#troubleshooting)
- [License](#license)

---

## Overview

This website serves as the online presence for the Zhan/Jin Laboratory at Zhejiang University School of Medicine. The site showcases research in cancer neuroscience, cancer immunology, CAR-T cell therapy, glioblastoma, and neuro-oncology.

**Live URL** (after deployment): `https://your-org-name.github.io` or `https://username.github.io/repo-name`

## Features

- ✨ Clean, modern academic design
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎨 Professional color scheme with excellent readability
- 📚 YAML-based publication management
- 📰 Jekyll blog system for news/updates
- 🖼️ Photo gallery structure
- 🔍 SEO-friendly
- 🚀 Free hosting via GitHub Pages
- ⚡ Fast loading, no heavy dependencies

## Getting Started

### Prerequisites

To run the site locally, you need:

- **Ruby** (version 2.7 or higher)
- **Bundler** (`gem install bundler`)
- **Git**

Check your Ruby version:
```bash
ruby -v
```

If you don't have Ruby installed:
- **macOS**: Ruby comes pre-installed, or use `brew install ruby`
- **Linux**: Use your package manager (e.g., `sudo apt-get install ruby-full`)
- **Windows**: Download from [RubyInstaller](https://rubyinstaller.org/)

### Local Development

1. **Navigate to the website directory:**
   ```bash
   cd zhanjin-lab-website
   ```

2. **Install dependencies:**
   ```bash
   bundle install
   ```

3. **Run the local development server:**
   ```bash
   bundle exec jekyll serve
   ```

4. **Open your browser** and go to:
   ```
   http://localhost:4000
   ```

5. **Making changes**: The site will automatically rebuild when you save files. Refresh your browser to see changes.

**Note**: If you modify `_config.yml`, you need to restart the server.

---

## GitHub Pages Deployment

### Option 1: Organization Account (Recommended)

This option creates a more professional URL and makes it easier to transfer ownership.

#### Step 1: Create a GitHub Organization

1. Go to [GitHub](https://github.com) and click the **+** icon → **New organization**
2. Choose a name (e.g., `zhanjin-lab`, `zju-neuroonc-immuno`)
3. Complete the setup

#### Step 2: Create Repository

1. In your organization, click **New repository**
2. Name it exactly: `<org-name>.github.io` (e.g., `zhanjin-lab.github.io`)
3. Make it **Public**
4. Do NOT initialize with README (we already have one)
5. Click **Create repository**

#### Step 3: Push Your Code

```bash
cd zhanjin-lab-website
git init
git add .
git commit -m "Initial commit: Zhan/Jin Lab website"
git branch -M main
git remote add origin https://github.com/your-org-name/your-org-name.github.io.git
git push -u origin main
```

#### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in the left sidebar)
3. Under "Source", select:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
4. Click **Save**

**Your site will be live at**: `https://your-org-name.github.io` (usually within 1-2 minutes)

---

### Option 2: Personal Account

If you prefer to start with your personal account:

#### Step 1: Create Repository

1. Go to GitHub and click **New repository**
2. Choose a name (e.g., `zhanjin-lab-website`)
   - For URL `username.github.io`, name must be exactly that
   - For URL `username.github.io/repo-name`, any name works
3. Make it **Public**
4. Click **Create repository**

#### Step 2: Push Your Code

```bash
cd zhanjin-lab-website
git init
git add .
git commit -m "Initial commit: Zhan/Jin Lab website"
git branch -M main
git remote add origin https://github.com/username/repo-name.git
git push -u origin main
```

#### Step 3: Enable GitHub Pages

Same as Option 1, Step 4.

If using a project repository (not `username.github.io`), update `_config.yml`:
```yaml
baseurl: "/repo-name"  # e.g., "/zhanjin-lab-website"
```

---

## Content Management

### Adding Publications

Publications are stored in YAML files: `_data/publications_zhan.yml` and `_data/publications_jin.yml`.

**To add a new publication:**

1. Open the appropriate YAML file
2. Find the correct year group or create a new one
3. Add the publication following this format:

```yaml
- year: 2025
  publications:
    - title: "Your publication title"
      authors: "Author1, Author2, Author3, [...], Last Author"
      journal: "Journal Name, Volume (Issue), Pages"
      citations: 10  # or null if not available
      doi: "10.1234/example"  # or null
      topic: "CAR-T"  # or "Glioblastoma", "Cancer Immunology", etc.
```

**Best practices:**
- Keep years in descending order (newest first)
- Use consistent formatting for author names
- Include full journal citation
- Update citation counts periodically
- Categorize by topic for future filtering

### Creating News Posts

News posts are markdown files in the `_posts/` directory.

**To create a new post:**

1. Create a file named: `YYYY-MM-DD-title.md` (e.g., `2025-12-15-new-publication.md`)
2. Add front matter and content:

```markdown
---
layout: post
title: "Your News Title"
date: 2025-12-15
---

Your news content goes here. Use markdown formatting:

- **Bold text**
- *Italic text*
- [Links](https://example.com)

## Subheadings

Paragraphs and more content...
```

3. Commit and push:

```bash
git add _posts/2025-12-15-new-publication.md
git commit -m "Add news post: new publication"
git push
```

**Filename rules:**
- Must start with date: `YYYY-MM-DD`
- Use hyphens, not spaces
- Must have `.md` extension

### Updating Team Members

Edit `people.md` to add, remove, or update team members.

**To add a new student:**

```markdown
<div class="team-member">
    <h3>Student Name</h3>
    <p class="title">Ph.D. Candidate, Zhejiang University School of Medicine</p>
    <p>Research focus: Brief description of research interests</p>
</div>
```

**To move a student to Alumni:**

1. Cut the student's entry from the current section
2. Paste it into the Alumni section
3. Update the title to indicate graduation

### Adding Photos

**To add photos to the gallery:**

1. Place images in `assets/images/` directory
2. Edit `photos.md`
3. Replace the "coming soon" section with:

```markdown
<div class="photo-grid">
    <div class="photo-item">
        <img src="{{ '/assets/images/photo1.jpg' | relative_url }}" alt="Lab group photo 2025">
        <p class="photo-caption">Lab meeting, March 2025</p>
    </div>
    <div class="photo-item">
        <img src="{{ '/assets/images/photo2.jpg' | relative_url }}" alt="Conference presentation">
        <p class="photo-caption">Dr. Jin presenting at CNS Conference 2025</p>
    </div>
</div>
```

**Image guidelines:**
- Optimize images before uploading (keep file sizes < 500KB)
- Use descriptive filenames (e.g., `lab-group-2025-03.jpg`)
- Recommended dimensions: 800-1200px wide
- Format: JPEG or PNG
- **Important**: Ensure no patient information or sensitive data is visible

---

## Customization

### Changing Colors

Edit `assets/css/style.css` in the `:root` section:

```css
:root {
    --primary-color: #2563eb;      /* Main accent color */
    --primary-dark: #1e40af;       /* Darker shade for hover */
    --text-dark: #1f2937;          /* Main text color */
    /* ... */
}
```

### Updating Contact Information

Edit `_config.yml`:

```yaml
lab:
  name: "Your Lab Name"
  institution: "Your Institution"
  location: "Your Address"
  email: "your-email@university.edu"
```

### Modifying Navigation

Edit `_includes/navigation.html` to add, remove, or reorder menu items.

### Adding Google Analytics (Optional)

1. Get your Google Analytics tracking ID
2. Add to `_config.yml`:
   ```yaml
   google_analytics: UA-XXXXXXXXX-X
   ```
3. Create `_includes/analytics.html` with your tracking code
4. Include it in `_layouts/default.html` before `</head>`

---

## Troubleshooting

### Site Not Building on GitHub Pages

**Check:**
1. Repository is public
2. Branch is set to `main` in Pages settings
3. No syntax errors in `_config.yml`
4. All required files are present

**View build errors:**
- Go to repository → **Actions** tab
- Click on the latest workflow run

### Local Development Issues

**"Could not find gem" error:**
```bash
bundle install
bundle update
```

**"Permission denied" error:**
```bash
sudo gem install bundler
```

**Site not updating:**
- Clear browser cache
- Hard refresh (Cmd+Shift+R / Ctrl+Shift+R)
- Check that `_site/` is in `.gitignore` (it should be)

### Images Not Showing

- Check file paths use `{{ '/assets/images/file.jpg' | relative_url }}`
- Ensure images are committed to git
- Verify image files are not ignored by `.gitignore`

---

## Site Structure

```
zhanjin-lab-website/
├── _config.yml              # Site configuration
├── _layouts/                # Page templates
│   ├── default.html
│   ├── page.html
│   └── post.html
├── _includes/               # Reusable components
│   ├── header.html
│   ├── navigation.html
│   └── footer.html
├── _data/                   # Data files
│   ├── publications_zhan.yml
│   └── publications_jin.yml
├── _posts/                  # News/blog posts
│   └── 2025-12-06-welcome-to-zhanjin-lab.md
├── assets/                  # Static assets
│   ├── css/
│   │   └── style.css
│   ├── images/
│   └── js/
├── index.md                 # Home page
├── research.md              # Research page
├── people.md                # People/Team page
├── publications.md          # Publications page
├── news.md                  # News listing page
├── photos.md                # Photo gallery page
├── contact.md               # Contact page
├── Gemfile                  # Ruby dependencies
└── README.md                # This file
```

---

## Updating the Site (Quick Reference)

**Add a news post:**
```bash
# Create file: _posts/YYYY-MM-DD-title.md
git add _posts/
git commit -m "Add news post"
git push
```

**Add publications:**
```bash
# Edit: _data/publications_jin.yml or _data/publications_zhan.yml
git add _data/
git commit -m "Update publications"
git push
```

**Update any page content:**
```bash
# Edit the .md file
git add .
git commit -m "Update [page name]"
git push
```

Changes will be live on your GitHub Pages site within 1-2 minutes.

---

## Migrating to an Organization Later

If you start with a personal account and want to move to an organization:

1. Create the organization on GitHub
2. Transfer the repository (Settings → Transfer ownership)
3. Update the repository name if needed
4. Re-enable GitHub Pages in the new repository settings
5. Update any hardcoded URLs in your content

---

## Maintenance Checklist

**Monthly:**
- [ ] Update publication citation counts
- [ ] Add new publications
- [ ] Post lab news/updates

**Quarterly:**
- [ ] Review and update team member info
- [ ] Add new photos from events
- [ ] Check for broken links

**Annually:**
- [ ] Update copyright year in footer
- [ ] Review all content for accuracy
- [ ] Update Ruby/Jekyll dependencies (`bundle update`)

---

## Support & Documentation

- **Jekyll Documentation**: https://jekyllrb.com/docs/
- **GitHub Pages**: https://docs.github.com/en/pages
- **Markdown Guide**: https://www.markdownguide.org/
- **YAML Syntax**: https://yaml.org/

---

## License

This website template is created for the Zhan/Jin Laboratory. Feel free to adapt it for your own academic lab website.

---

## Contact

For questions about this website:
- Dr. Jin Linchun: linchun.jin@zju.edu.cn
- Laboratory: 1196057@zju.edu.cn

---

**Version**: 1.0  
**Last Updated**: December 2025  
**Built with**: Jekyll 4.3 + GitHub Pages

