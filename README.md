# Juhyeok Lee | Academic Website

Personal academic website for Juhyeok Lee, hosted on GitHub Pages.

- Website: https://jhyeoklee.github.io/
- Repository: https://github.com/jhyeoklee/jhyeoklee.github.io
- Publishing branch: `main`
- Publishing folder: repository root

## Site content

The navigation and page sections follow this order:

1. About
2. Publications
3. Research, with separate Working Papers and Work in Progress groups
4. Teaching
5. CV

Edit `index.html` for content and `assets/css/style.css` for styling.
Replace `files/Juhyeok_Lee_CV.pdf` to update the CV download, and update the
date shown in the CV section. The October 2026 CV is included.

## Update the website

For a fresh local copy:

```sh
git clone https://github.com/jhyeoklee/jhyeoklee.github.io.git
cd jhyeoklee.github.io
```

Before editing an existing copy, pull the latest changes:

```sh
git pull --ff-only origin main
```

After editing and reviewing the website:

```sh
git add index.html assets/css/style.css files/Juhyeok_Lee_CV.pdf
git commit -m "Update academic website"
git push origin main
```

GitHub may ask you to sign in when pushing from a new computer.
Commits pushed to `main` are published automatically by the existing GitHub
Pages configuration. Track deployment under the repository's Actions tab.

## Preview locally

Open `index.html` in a browser, or run the following from the repository folder:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Then visit http://127.0.0.1:8000/.

This is a static HTML/CSS website. The `.nojekyll` file tells GitHub Pages to
serve the site without Jekyll processing.
