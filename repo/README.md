# Ayush Singh — Portfolio

Static, multi-page site. No build step, no framework — plain HTML/CSS/JS,
so GitHub Pages can serve it directly.

## Structure
```
index.html       About
portfolio.html   Stats, engagements, projects, client marquee
resume.html      Full resume + PDF download
contact.html     Contact links
terminal.html    Interactive command-line easter egg
assets/
  css/style.css  Shared styles (dark/light theme)
  js/main.js     Theme toggle + active-nav highlighting
  img/profile.jpg
  resume.pdf     Downloadable resume (swap this file to update it)
```

## Run locally
Just open `index.html` in a browser — no server required. (Or run
`python3 -m http.server` from this folder and visit `localhost:8000`.)

## Deploy on GitHub Pages
1. Create a new GitHub repo and push this folder as its contents:
   ```
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
2. On GitHub: **Settings → Pages → Source → Deploy from a branch →
   `main` / `/ (root)`** → Save.
3. Your live URL will be `https://<your-username>.github.io/<repo-name>/`.
   Wait 1–2 minutes after the first push for it to go live.

## To update content
- Resume text: edit `resume.html` directly.
- Resume PDF: replace `assets/resume.pdf` with a new export (keep the filename).
- Profile photo: replace `assets/img/profile.jpg` (keep it square, ideally ≥600×600).
- Client/engagement list: edit the `clients` array in `portfolio.html`.
