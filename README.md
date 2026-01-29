# Farhat Binte Azam — Academic Website (GitHub Pages)

This is a fast, professional academic website built with **Jekyll + Minimal Mistakes** and designed for **R1 faculty / postdoc / postdoc-to-faculty** searches.

## Quick start (local preview - optional)
1. Install Ruby + Bundler (macOS: `brew install ruby` then `gem install bundler`)
2. Run:
   - `bundle install`
   - `bundle exec jekyll serve`
3. Open http://localhost:4000

## One-click deploy (recommended)
1. Create a GitHub repo named: **<your-username>.github.io**
2. Upload all files from this folder to the repo root.
3. GitHub → **Settings → Pages**
   - Source: **Deploy from a branch**
   - Branch: **main / (root)**
4. Your site will be live at: https://<your-username>.github.io

## Custom domain (farhatazam.com)
1. In GitHub → Settings → Pages:
   - Add **Custom domain**: `farhatazam.com`
   - Enable **Enforce HTTPS**
2. In your domain DNS settings, add:
   - A records for `@` to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Optional (recommended): CNAME for `www` → `<your-username>.github.io`
3. Add a file named `CNAME` at repo root containing:
   - `farhatazam.com`

## Update content
Edit the markdown files in `_pages/` and `index.md`.
- CV PDF: `assets/pdf/CV_Farhat_Binte_Azam.pdf`
