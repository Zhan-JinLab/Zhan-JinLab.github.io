# Deployment Checklist

Use this checklist to ensure smooth deployment of your lab website.

## Pre-Deployment

- [ ] Review all content for accuracy
- [ ] Check that email addresses are correct in `_config.yml` and `contact.md`
- [ ] Verify team member information in `people.md`
- [ ] Review publication data in `_data/publications_*.yml`
- [ ] Test site locally with `bundle exec jekyll serve`
- [ ] Check all internal links work
- [ ] Ensure no placeholder text remains (search for "TODO", "coming soon", etc.)

## GitHub Setup

- [ ] Create GitHub organization (recommended) or decide on personal account
- [ ] Create repository with correct name:
  - Organization: `org-name.github.io`
  - Personal: `username.github.io` or any name for project site
- [ ] Make repository public
- [ ] Add repository description and website URL

## Code Push

- [ ] Initialize git repository (`git init`)
- [ ] Add all files (`git add .`)
- [ ] Create initial commit
- [ ] Set branch to main (`git branch -M main`)
- [ ] Add remote origin
- [ ] Push to GitHub (`git push -u origin main`)

## GitHub Pages Configuration

- [ ] Go to repository Settings → Pages
- [ ] Set source to `main` branch, `/` (root) folder
- [ ] Save settings
- [ ] Wait 1-2 minutes for build
- [ ] Visit your site URL

## Post-Deployment Checks

- [ ] Site loads correctly at your GitHub Pages URL
- [ ] All pages are accessible from navigation
- [ ] Images load properly (if any added)
- [ ] Links work (internal and external)
- [ ] Responsive design works on mobile (test with browser dev tools)
- [ ] Check different browsers (Chrome, Firefox, Safari)

## Configuration Updates (If Needed)

- [ ] If using project repository (not org.github.io), update `baseurl` in `_config.yml`
- [ ] Custom domain? Add CNAME file and configure DNS (see GitHub docs)

## Optional Enhancements

- [ ] Add Google Analytics tracking ID
- [ ] Set up custom domain (requires DNS configuration)
- [ ] Add social media links to footer
- [ ] Create favicon (place in `assets/images/` and reference in `default.html`)
- [ ] Add Open Graph meta tags for better social sharing

## Share Your Site

- [ ] Update lab email signature with website URL
- [ ] Add to institutional directory
- [ ] Share with lab members
- [ ] Update Google Scholar profiles
- [ ] Add to ResearchGate, Twitter/X bio, etc.

## Ongoing Maintenance

- [ ] Schedule monthly content updates
- [ ] Assign someone to manage news posts
- [ ] Set reminder to update publications quarterly
- [ ] Review team page when members join/leave
- [ ] Keep Ruby gems updated annually (`bundle update`)

---

## Troubleshooting

**Site not building?**
- Check repository Actions tab for build errors
- Verify `_config.yml` syntax
- Ensure all required files are present

**404 errors?**
- Check `baseurl` in `_config.yml`
- Verify file paths use `{{ '/path' | relative_url }}`

**Changes not showing?**
- Wait 1-2 minutes for GitHub rebuild
- Clear browser cache
- Check commit was pushed successfully

---

## URLs to Bookmark

- [ ] Live site: `https://______.github.io`
- [ ] GitHub repository: `https://github.com/______/______`
- [ ] Repository settings: `https://github.com/______/______/settings`

---

**Deployment Date**: ___________  
**Deployed By**: ___________  
**Site URL**: ___________

