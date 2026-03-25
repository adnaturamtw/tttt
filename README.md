# AromaFonda Website

A clean, elegant, responsive multi-page website for **AromaFonda** (wellness/aromatherapy brand), built with static HTML/CSS/JS for easy GitHub Pages deployment.

## Project Structure

```text
.
├── index.html                    # Home / 首頁
├── about.html                    # About / 關於 AromaFonda
├── olfactory-analysis.html       # Japanese Olfactory Analysis / 日本嗅覺反應分析
├── courses.html                  # Courses / 健康課程
├── ad-naturam.html               # Ad Naturam
├── contact.html                  # Contact / 聯絡我們
├── assets/
│   ├── css/
│   │   └── site.css              # Shared styling, responsive layout, color system
│   └── js/
│       └── site.js               # Mobile menu interaction
└── images/                       # Existing image assets (optional use)
```

## Run Locally

Because this is a static site, you can open `index.html` directly, or run a local server:

```bash
python3 -m http.server 8000
```

Then visit: `http://localhost:8000`

## Deploy to GitHub Pages

### Option A: Deploy from root (recommended)
1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source**: Deploy from a branch
   - **Branch**: `main` (or your default branch)
   - **Folder**: `/ (root)`
4. Save and wait for deployment.

### Option B: Use existing workflow
If this repo already has a GitHub Actions workflow for static publishing, keep it enabled and push changes to trigger deployment.

## Where to Edit Text Later

- **Homepage text**: `index.html`
- **About page text**: `about.html`
- **Analysis page text**: `olfactory-analysis.html`
- **Courses text**: `courses.html`
- **Ad Naturam text**: `ad-naturam.html`
- **Contact text and form fields**: `contact.html`
- **Global colors/spacing/typography**: `assets/css/site.css`
- **Mobile navigation behavior**: `assets/js/site.js`

## Notes

- The contact form is currently front-end only.
- A comment in `contact.html` marks where to connect Formspree/Netlify Forms/custom backend later.
