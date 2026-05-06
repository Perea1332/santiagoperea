# Santiago Perea — Personal Academic Website

Built with [Quarto](https://quarto.org/) and deployed to GitHub Pages.

## Project Structure

```
.
├── _quarto.yml          # Site configuration (title, navbar, theme)
├── index.qmd            # Home / About page
├── research.qmd         # Research projects
├── publications.qmd     # Full publication list
├── teaching.qmd         # Teaching & mentorship
├── outreach.qmd         # Outreach & press coverage
├── contact.qmd          # Contact page
├── styles.css           # Custom CSS (colors, cards, layout)
├── images/              # Put your profile photo here
│   └── profile.jpg      # ← Your headshot goes here!
├── docs/                # Rendered output (auto-generated, served by GitHub Pages)
└── .github/
    └── workflows/
        └── publish.yml  # GitHub Actions: auto-render & deploy on push
```

## Quick Start

### Prerequisites
- [R](https://www.r-project.org/) (≥ 4.0)
- [Quarto](https://quarto.org/docs/get-started/) (≥ 1.4)
- [RStudio](https://posit.co/download/rstudio-desktop/) (recommended)

### Preview locally

```bash
# In the project folder:
quarto preview
```

This opens a live-reloading local preview at `http://localhost:4848`.

### Add your photo

1. Save your headshot as `images/profile.jpg`  
2. Open `index.qmd` and find the comment `<!-- Replace the emoji below...`  
3. Replace the `<div class="profile-placeholder">` block with:

```html
<img src="images/profile.jpg" class="profile-photo" alt="Santiago Perea">
```

### Render the site

```bash
quarto render
```

Output goes to `docs/`. This is what GitHub Pages will serve.

## Deploying to GitHub Pages

### Option A — Automatic (GitHub Actions) ⭐ Recommended

1. Push this folder to a new GitHub repository
2. Go to **Settings → Pages**
3. Set **Source** to **GitHub Actions**
4. Every `git push` to `main` will automatically render and deploy your site

Your site will be live at: `https://[your-username].github.io/[repo-name]/`

### Option B — Manual (render locally, push docs/)

1. Run `quarto render` locally
2. Commit and push the `docs/` folder to GitHub
3. Go to **Settings → Pages → Source: Deploy from branch → main / docs/**

## Customization Tips

### Change colors
Edit the `:root` block at the top of `styles.css`:
```css
:root {
  --forest-dark:  #1b4332;   /* Navbar, headings */
  --forest-mid:   #2d6a4f;   /* Links, accents */
  --forest-pale:  #74c69d;   /* Tags, borders */
}
```

### Add pages
1. Create a new `.qmd` file (e.g., `cv.qmd`)
2. Add it to the `navbar:` section in `_quarto.yml`

### Update publications
Edit `publications.qmd` — each publication follows the pattern:
```html
<div class="pub-item">
  <div class="pub-authors">Author, A., & Author, B.</div>
  <div class="pub-title">Title of the paper.</div>
  <div class="pub-journal">
    <em>Journal Name</em>, vol(issue), pages.
    <a href="https://doi.org/..." target="_blank">DOI</a>
  </div>
</div>
```

### Link a custom domain
If you have a domain (e.g., `santiagoperea.com`):
1. Go to **Settings → Pages → Custom domain**
2. Add a file named `CNAME` to this folder containing just your domain name

## Need help?

- [Quarto documentation](https://quarto.org/docs/websites/)
- [GitHub Pages docs](https://docs.github.com/en/pages)
