# PHY308 — Mechanics of Discrete & Continuous Systems

## Fall 2026 — Prof. Daniel Grin — Haverford College

This is the course website for PHY308, built as a single-page HTML site with 9 tabbed sections.

### Structure

| File | Purpose |
|------|---------|
| `index.html` | The entire site (vanilla HTML/CSS/JS, no frameworks required) |
| `catenoid.jpeg` | Catenoid image used in the About tab |
| `PHY308Syllabus_Fall2026.pdf` | Downloadable PDF of the full syllabus |
| `README.md` | This file |

### 9 Tabs

| Tab | Content |
|-----|---------|
| **About** | Motivation + catenoid image + course info box + link to PDF syllabus |
| **Schedule** | Full 14-week draft schedule as a responsive table |
| **Course Structure** | Thursday lecture format + Tuesday collaborative problem-solving |
| **Materials** | Required texts, supplementary books, how to read the textbook |
| **Assignments & Grading** | Homework, Python problems, Exams/Quizzes, Grading breakdown |
| **Participation** | Concept tests, Piazza, group collaboration, how it fits into your grade (14%) |
| **Policies** | Late work policy + full Honor Code (collaboration, Mathematica, AI, references) |
| **Classroom Norms** | Values statement, APS code of conduct, Title IX / college policies |
| **Resources & Support** | Communication, OAR, Accessibility / ADS |

### Design

- Haverford red (`#981e32`) accent color
- Sticky navigation bar with 9 tabs fitting in one row
- TA names displayed in the header masthead
- Catenoid image in the About tab
- "Syllabus" label in italics under the professor name
- Downloadable PDF link at the bottom of the About tab
- Responsive layout (works on mobile)
- URL hash routing (`#schedule`, `#policies`, etc.) — bookmarkable tabs
- Callout boxes for important notes
- Hover-highlighted schedule rows

### Footer

Site design based on Andrea Lommen's Physics/Astro 104 page. Advice from Ted Brzinski. Generated with DeepSeek V4 Pro 0423.

### Editing TA Office Hours

TA office hours can be added by editing the `index.html` file. Look for the TA line in the header:

```html
<div class="tas">Teaching Assistants: Joey Busch, Viraj Singhania, Heshu Yin</div>
```

To add office hours, simply extend this line, e.g.:

```html
<div class="tas">Teaching Assistants: Joey Busch (Mon 2–4), Viraj Singhania (Wed 3–5), Heshu Yin (Fri 1–3)</div>
```

### Deploying to GitHub Pages

1. Create a new GitHub repository (e.g., `PHY308`)
2. Push the contents of this `site/` folder to the repository:

```bash
cd site
git init
git add index.html catenoid.jpeg PHY308Syllabus_Fall2026.pdf README.md
git commit -m "Initial commit: PHY308 course website"
git branch -M main
git remote add origin git@github.com:YOURUSERNAME/PHY308.git
git push -u origin main
```

3. Go to the repository on GitHub → **Settings** → **Pages**
4. Under "Branch", select `main` and `/ (root)`, then click **Save**
5. The site will be live at: `https://YOURUSERNAME.github.io/PHY308/`

### Local Preview

Since this is a static HTML file, you can preview it locally by simply opening `index.html` in any browser:

```bash
open index.html
```

No server, build step, or framework needed.