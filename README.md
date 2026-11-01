# ZenPortfolio

Hi, I'm **Zenith Saru**, a civil engineer from Kathmandu, Nepal. This is the source for my personal portfolio website.

**Live site:** https://zenithsaru.github.io/ZenPortfolio/

I'm not a web developer. I wanted a portfolio that looked like it belonged to a civil engineer, so the whole site is laid out like a set of engineering drawings, with sheet borders, title blocks and sheet numbers. If you've stumbled on this repo and want something similar for yourself, you're welcome to use it as a starting point. Below is everything I wish I'd known when I started.

---

## Why it might be useful to you

- **It's one file.** Everything lives in `index.html`. There's no framework, no `npm install` and no build step.
- **It's free to host.** It runs on GitHub Pages, so you don't need a server or a domain.
- **It's easy to edit.** Each section is clearly marked, so you can change it with any text editor.
- **It works on phones** and prints cleanly, in case someone (a professor, for example) wants a paper copy.

## Making it your own

1. **Get a copy.** Click **Fork** at the top of this page, or **Code → Download ZIP**.
2. **Open `index.html`** in a text editor. [VS Code](https://code.visualstudio.com/) is free and makes this easier.
3. **Change the name in the title block.** Near the top there's a small block marked `EDIT HERE`. It controls the name and "last updated" date shown on every sheet.
4. **Edit each section.** They're marked with comments like this:
   ```html
   <!-- ================= 03 EDUCATION ================= -->
   ```
   | Section | What's in it |
   |---|---|
   | `01 INTRODUCTION` | Name, short statement, photo, contact links |
   | `02 RESEARCH INTERESTS` | Your motivation, areas of interest, key numbers |
   | `03 EDUCATION` | Degree, thesis, advisor, coursework |
   | `04 PROJECTS` | One `<article class="proj">` block per project |
   | `05 PUBLICATIONS` | Papers and presentations |
   | `06 EXPERIENCE` | Jobs and positions (table rows) |
   | `07 SKILLS & LEADERSHIP` | Software, languages, activities |
   | `08 CONTACT` | Email, phone, profiles |
5. **Swap in your files.** Put your photo and project images in the `images/` folder and your CV in the main folder as `cv.pdf`. Use simple file names without spaces (`thesis-map.jpg`, not `Fig 1.jpg`). Spaces in file names break links on the web.
6. **Remove what you don't need.** To drop a section (no publications yet is completely fine), delete its `<section>` block **and** its link in the top menu (`<nav aria-label="Sections">`).
7. **Check it.** Double-click `index.html` to open it in your browser, and refresh after each save.

**Please replace all of my content with your own:** my photo, CV, text and project images. The layout is yours to use; my details aren't.

## Putting it online (free)

1. Push your copy to a **public** GitHub repository.
2. Go to **Settings → Pages**.
3. Under "Build and deployment", choose **Deploy from a branch**, then select **main** and **/ (root)**, and click Save.
4. After a minute or two your site is live at `https://<your-username>.github.io/<repo-name>/`.

Every time you push a change, the site updates by itself.

> **Want the repo private?** GitHub Pages needs a public repo on a free account. [Netlify](https://www.netlify.com/) and [Cloudflare Pages](https://pages.cloudflare.com/) can host straight from a private repo for free. Keep in mind that whatever the site shows (including your CV) is public either way.

## Updating it later

From the project folder:

```bash
git pull
git add .
git commit -m "Update portfolio"
git push
```

Run `git pull` first if you've edited anything on the GitHub website, so your computer and GitHub stay in sync.

## What it's built with

- Plain HTML and CSS, plus a few lines of JavaScript that draw the sheet borders and title blocks
- Fonts: [Figtree](https://fonts.google.com/specimen/Figtree) and [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) from Google Fonts

## Say hi

If this helped you, or you're a fellow engineer working on remote sensing, hydrology or machine learning, I'd love to hear from you.

- Email: zenithsaru@gmail.com
- LinkedIn: [zenith-saru-26726b3b4](https://www.linkedin.com/in/zenith-saru-26726b3b4)
- ORCID: [0009-0001-1701-7023](https://orcid.org/0009-0001-1701-7023)

Good luck with your own portfolio.
