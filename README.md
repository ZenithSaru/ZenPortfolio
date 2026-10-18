# ZenPortfolio

Personal portfolio website for a civil engineer, designed like a set of engineering drawings. It's a single page: everything lives in `index.html`, with no build step and no dependencies.

## Editing

Open `index.html` in any text editor (VS Code is a good free choice). Each section is marked with a comment like `<!-- ================= 03 EDUCATION ================= -->`.

| What | Where |
|---|---|
| Name and "last updated" shown in every title block | The `SET` block near the top, marked `EDIT HERE` |
| Name, statement, contact facts | Section `01 INTRODUCTION` |
| Research interests and key numbers | Section `02 RESEARCH INTERESTS` |
| Degree, GPA, thesis, advisor, coursework | Section `03 EDUCATION` |
| Projects (one `<article class="proj">` each) | Section `04 PROJECTS` |
| Papers and presentations | Section `05 PUBLICATIONS` |
| Jobs | Section `06 EXPERIENCE` (table rows) |
| Skills, certifications, awards | Section `07 SKILLS & AWARDS` |
| Email, phone, links | Section `08 CONTACT` |

To remove a section, delete its `<section>` block **and** its link in the top menu (`<nav aria-label="Sections">`).

### Files to add

- `cv.pdf`: your CV, linked from the top bar and contact section.
- `images/headshot.jpg`: replace `<span>YN</span>` in the photo box with `<img src="images/headshot.jpg" alt="Your Name">`.
- Project images: replace the `<svg>…</svg>` inside a `.fig` box with `<img src="images/your-photo.jpg" alt="Short description">`.

## Previewing

Double-click `index.html` to open it in your browser. Refresh after each save.

## Publishing changes

```bash
git add .
git commit -m "Update portfolio"
git push
```

The site is published with GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / root**. It will be live at `https://zenithsaru.github.io/ZenPortfolio/`.
