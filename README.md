# My Resume Website: CSS Project

**Preetam Pradhan** | **Roll No: 26120969** | Web Development Mid-Term Project  
🎓 Dual-Degree Student at **NMIMS** (B.Com Honours) & **IIM Bangalore** (BBA-DB&E)

---

### 🌐 Quick Links & Badges

| Resource | Link |
| :--- | :--- |
| 🚀 **Live Website (GitHub Pages)** | [https://preetampradhan.github.io/resume/](https://preetampradhan.github.io/resume/) |
| 📁 **GitHub Repository** | [https://github.com/preetampradhan/resume](https://github.com/preetampradhan/resume) |
| ✉️ **Contact Email** | [pallapreetpradhan@gmail.com](mailto:pallapreetpradhan@gmail.com) |

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive Design](https://img.shields.io/badge/Responsive-Mobile%20%7C%20Tablet%20%7C%20Desktop-2457f5?style=for-the-badge)
![GitHub Pages](https://img.shields.io/badge/Hosted%20On-GitHub%20Pages-222222?style=for-the-badge&logo=github)

---

## 1. About My Website
This is my personal resume and portfolio website. In the HTML module, I built the structural semantic foundation of the page, and in this project, I used modern CSS to style and transform it into a recruiter-friendly, premium experience.

I am a first-year dual-degree student at **NMIMS** (B.Com Honours) and **IIM Bangalore** (BBA-Digital Business and Entrepreneurship, BBA-DB&E), looking for an analysis or management internship. I engineered the site for recruiters and academic evaluators so they can rapidly find my academic credentials, leadership background, and technical skills.

The project is kept ultra-clean with zero unnecessary dependencies, organized across:
- `index.html` — Clean semantic HTML5 markup
- `style.css` — Custom responsive CSS3 design system
- `README.md` — Project documentation and assignment overview

---

## 2. Sections of My Website

- **Navigation Bar**: Six smooth-scrolling links (`Home`, `Experience`, `Education`, `Skills`, `Resume`, `Contact`). Made sticky to remain pinned at the top with glassmorphic backdrop blur and an animated scroll progress line that fills across the header as the user scrolls down.
- **Hero Section**: Prominent name display, dynamic animated "Open to internships" status pill with a pulsating green radar dot, student Roll No (`26120969`), concise career summary, direct action buttons (Email, LinkedIn, GitHub, and Print Resume), and a 3-item CSS Grid facts row highlighting **95.8% in Class 12**, **School Pupil Leader**, and **Two degrees**.
- **01 Experience**: Structured vertical timeline with two panels highlighting leadership as **School Pupil Leader** (managing 1,400+ students and coordinating events) and team excellence in **Debate and indoor events**.
- **02 Education**: Elegant card list displaying **Indian Institute of Management Bangalore**, **NMIMS**, and **SAI International School, Bhubaneswar (CBSE)** with academic score badges.
- **03 Skills**: Four modern CSS Grid tiles covering **Team leadership**, **Event coordination**, **Public speaking & debate**, and **Mentoring**, complete with hover lifts and accent indicators.
- **04 Resume**: A paper-style sheet with realistic layered drop-shadows and contact metadata. It includes an interactive **Print / PDF** button and dedicated print media styles so that when printed or saved as PDF, it renders as a clean black-and-white A4 single-page resume.
- **Contact & Footer**: Full-width dark navy band featuring a dot-matrix background, glowing accent geometry, large accessible email hyperlink, and a footer with smooth Back-to-Top navigation.

---

## 3. What I Did with CSS

### Typography & Fonts
- Headings: **Fraunces** (Google Fonts variable serif) for confident, professional, and academic typography.
- Body: **Figtree** (Google Fonts sans-serif) for high legibility across screens of all sizes.

### Colour System (CSS Variables)
Saved as reusable tokens in `:root`:
- Deep Navy: `#0e1a36` (Primary dark background and headings)
- Vibrant Royal Blue: `#2457f5` (Accent colour for buttons, lines, and active states)
- Light Sky Blue: `#9db8ff` (Highlights, borders, and pills)
- Cool Soft Grey: `#f4f7fc` (Secondary section background)
- Surface White: `#ffffff` (Card background)

### CSS Layout & Modern Properties
- **Positioning**: `position: sticky` with `top: 0` for the persistent nav bar; `position: absolute` for the vertical timeline rail, glowing timeline bullet nodes, and decorative orbital background geometry.
- **CSS Grid & Flexbox**:
  - `display: flex` for the sticky navigation bar, action button groups, education cards, and footer.
  - `display: grid` for the 3-column hero facts row and the 2x2 skills tiles.
- **Full-Width Section Bands**: Dark hero/contact bands and light experience/skills bands stretch across 100% of the viewport width using `box-shadow: 0 0 0 100vmax ...` and `clip-path: inset(0 -100vmax)` while keeping text cleanly centered inside `.wrap`.
- **CSS Selectors**:
  - Element selectors (`body`, `h1`, `h2`, `h3`, `p`, `ul`, `li`, `mark`, `footer`)
  - Class selectors (`.card`, `.nav-link`, `.facts`, `.skill-tile`, `.edu-card`, `.text-link`)
  - ID selectors (`#hero`, `#experience`, `#education`, `#skills`, `#resume-top`, `#resume`, `#contact`)
  - Pseudo-classes & pseudo-elements (`:hover`, `:focus-visible`, `::before`, `::after`, `::selection`)
- **Automated Section Numbering**: CSS counters (`counter-reset: sec;` and `counter-increment: sec;`) with `content: counter(sec, decimal-leading-zero)` to automatically generate standard `01`, `02`, `03`, `04` section markers.
- **Spacing & Alignment**: A `.wrap` container with `max-width: 65ch` on paragraphs to ensure optimal readability, responsive fluid scaling with `clamp()`, and smooth scrolling (`scroll-behavior: smooth`).

---

## 4. Making It Work on Every Device (Responsive & Accessible)

- **Responsive Breakpoints**:
  - `1600px+` (Large high-resolution desktop screens)
  - `1100px` (Standard desktop monitors)
  - `860px` (Tablets — collapses facts grid, hides decorative background rings to prevent obstruction)
  - `700px` (Smartphones — single column card layout, full-width touch buttons, horizontal scrollable navigation bar with subtle fade mask)
  - `380px` (Small smartphones — scaled typography and compact padding)
  - Landscape orientation (`max-height: 500px`) — disables sticky header to maximize vertical screen area.
- **Touch Targets & Hover**: Hover lifts and shadows are active only on pointer devices (`@media (hover: hover)`), while touch devices receive tap targets of at least `44px` height.
- **Accessibility**:
  - Clear `:focus-visible` outlines for keyboard navigability.
  - High WCAG AA+ contrast ratios between text and background.
  - Respects user accessibility preferences through `@media (prefers-reduced-motion: reduce)` which disables animations.
- **Print Stylesheet (`@media print`)**:
  - Strips away navigation, hero, background textures, buttons, and footer.
  - Formats the `#resume` section into a pristine single-page A4 document ready for PDF export.

---

## 5. Repository Structure

```
├── index.html       # Semantic HTML5 structure & content
├── style.css        # Professional Navy & Blue CSS stylesheet
└── README.md        # Comprehensive project documentation
```

---

## 6. How to Run Locally

1. Clone or download the repository:
   ```bash
   git clone https://github.com/preetampradhan/resume.git
   ```
2. Open `index.html` directly in any web browser, or serve it using Live Server:
   ```bash
   # Using VS Code: Right-click index.html -> "Open with Live Server"
   ```

---

## 7. GitHub Pages Deployment

1. The repository is published to GitHub under `preetampradhan/resume`.
2. Under **Settings > Pages**, the **Source** is set to **Deploy from a branch** (`main` / `root`).
3. The live deployment is available globally at:  
   **[https://preetampradhan.github.io/resume/](https://preetampradhan.github.io/resume/)**
