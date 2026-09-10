# Implementation Plan: Personal Developer Portfolio for Simran Kumari Keshri

Build a modern, sleek, high-converting, and responsive portfolio website for **Simran Kumari Keshri**, specializing in **Data Science, Java Backend Systems, and Full-Stack Engineering**.

The portfolio will feature a dark-mode aesthetic with ambient glow accents, glassmorphic surfaces, fluid micro-interactions, responsive navigation, live metric counters, interactive project cards, and a direct contact system.

---

## Proposed Architecture & Design System

### 1. Aesthetic & Design Tokens
- **Theme**: Deep obsidian/midnight backdrop (`#070a12`, `#0d1322`) with glassmorphism (`backdrop-filter: blur(16px)` and subtle borders `rgba(255, 255, 255, 0.08)`).
- **Accents**: Dual-gradient glowing accents — Electric Cyan (`#06b6d4`), Cyber Indigo (`#6366f1`), and Radiant Violet (`#a855f7`).
- **Typography**: 
  - Display & Headings: `Outfit` / `Plus Jakarta Sans` (punchy, modern, tech-forward)
  - Body & UI: `Inter` (clean, readable, highly legible)
  - Code & Badges: `JetBrains Mono` or `Fira Code` (developer authentic)
- **Visuals**: Realistic project preview mockups generated specifically for **Adigam AI** and **FoodConnect**, with no low-quality placeholders.

---

## User Review Required

> [!IMPORTANT]
> **Resume & Contact Details Confirmation**:
> - Email: `simrangrd373@gmail.com`
> - Phone: `+91 9693066314`
> - Location: `Bhopal, India`
> - Socials: 
>   - GitHub: [github.com/Simran-Keshri03](https://github.com/Simran-Keshri03)
>   - LinkedIn: [linkedin.com/in/simrankeshri](https://www.linkedin.com/in/simrankeshri)
>   - LeetCode: [leetcode.com/u/Simran_03/](https://leetcode.com/u/Simran_03/)
> - Resume Action: An interactive in-browser **Resume Modal Previewer** with a print/save as PDF trigger, plus standard direct download integration.

---

## Proposed Structure & Components

### 1. Header & Navigation (`<header>`, `<nav>`)
- Brand Logo: `<Simran/>` with an animated glowing dot indicator (`Available for Opportunities`).
- Nav Links: **About**, **Skills**, **Projects**, **Experience**, **Achievements**, **Contact**.
- Right Actions: "View Resume" modal button + "Get In Touch" accent CTA button.
- Mobile Hamburger Drawer: Seamless slide-out menu with smooth backdrop blur.

### 2. Hero Section (`#hero`)
- Availability Badge: `🟢 Open to Software Developer & Engineering Roles`
- Headline: `"Hi, I'm Simran Kumari Keshri"` with gradient highlight.
- Subheading: `"Software Developer & Data Science Specialist"`
- Bio Blurb: Emphasizing backend scalability (Java, Spring Boot), AI-powered applications, DSA problem solving (250+ LeetCode), and hackathon leadership.
- Action Buttons:
  - Primary: `"Explore Projects"` (smooth scroll to `#projects`)
  - Secondary: `"Contact Me"` (smooth scroll to `#contact`)
  - Ghost: `"Quick Resume"` (opens resume modal)
- Interactive Quick Social Dock: GitHub, LinkedIn, LeetCode, Email with hover popover tooltips.
- Interactive Background: Lightweight, fluid particle star-mesh canvas with mouse cursor repulsion/illumination.

### 3. Key Stats & Highlights (`#highlights`)
- **250+** LeetCode DSA Problems Solved (with direct profile link)
- **1st Place** HackInMotion 2026 Winner (EdTech Theme)
- **8.3** B.Tech CSE (Data Science) CGPA at LNCTE Bhopal
- **1st Prize** Graphic Design Competition (Creative & Visual UI/UX acumen)
- Animated rolling counter triggered on scroll view via `IntersectionObserver`.

### 4. Technical Skills Matrix (`#skills`)
Categorized tab/grid layout with category badges and skill level / technology pills:
- **Programming Languages**: Java, SQL
- **Backend & APIs**: Java Backend Development, Spring Boot, RESTful APIs, JWT Authentication
- **Frontend**: React, TypeScript, Modern CSS3/HTML5
- **Databases & Tools**: MySQL, Git, GitHub, VS Code
- **Core CS & Engineering**: Data Structures & Algorithms (DSA), OOPs, Database Management Systems (DBMS)

### 5. Featured Projects Showcase (`#projects`)
- Filter controls: `All`, `Full-Stack & Backend`, `AI & EdTech`.
- **Project 1: Adigam AI — AI-Powered Adaptive Learning Assistant**
  - HackInMotion 2026 Winner badge
  - Key capabilities: Learner performance analysis, dynamic mock tests, spaced repetition, AI doubt solver.
  - Tech tags: `React`, `TypeScript`, `AI Integration`, `REST APIs`
  - GitHub & Live Demo actions.
- **Project 2: FoodConnect — Waste-to-Welfare Logistics System**
  - Key capabilities: NGO & food donor bridge, real-time donation request tracking, surplus food distribution.
  - Tech tags: `Java`, `Spring Boot`, `React`, `MySQL`, `JWT`, `REST APIs`
  - GitHub & Live Demo actions.
- **GitHub Live Repository Banner**: Prompting visitors to explore more repositories directly at `Simran-Keshri03`.

### 6. Hackathons, Experience & Certifications (`#experience`)
- **HackInMotion 2026 Hackathon Winner (August 2026)**
  - 4-member team collaboration, lead frontend & assessment workflow engineering for Adigam AI.
- **Certifications & Training**:
  - *Java and Data Structures & Algorithms* — Sheriyans Coding School
  - *Virtual Internship Program (2026)* — ServiceNow University / AICTE & SmartBridge
  - *Essentials of Solution Development in IT (NSQF Level 5)* — SkillWallet Experiential Learning
- **Education Timeline**:
  - B.Tech in CSE (Data Science) — LNCTE Bhopal (CGPA: 8.3)
  - Higher Secondary Education — Jharkhand (78.4%)
  - Secondary Education — Jharkhand (90.8%)

### 7. Contact Section & Interactive Form (`#contact`)
- Contact cards with 1-click clipboard copy:
  - Email: `simrangrd373@gmail.com`
  - Phone: `+91 9693066314`
  - Location: `Bhopal, India`
- Direct Message Form:
  - Input validation for Name, Email, Subject, and Message.
  - Interactive submit animation with modern toast notification.
- Footer with copyright, back-to-top button, and social links.

### 8. Interactive Resume Modal (`#resume-modal`)
- Accessible `<dialog>` with modern `@starting-style` transitions for smooth top-layer entry and exit.
- Formatted digital resume preview with printable layout and download options.

---

## Proposed Changes

### Portfolio Directory (`d:\Portfolio`)

#### [NEW] [index.html](file:///d:/Portfolio/index.html)
Semantic HTML5 document containing all sections, SVG icons, metadata, OpenGraph tags, and structured schemas.

#### [NEW] [styles.css](file:///d:/Portfolio/styles.css)
Modular modern CSS with CSS variables, responsive flex/grid layouts, glassmorphism, animations, and top-layer dialog styling.

#### [NEW] [script.js](file:///d:/Portfolio/script.js)
Vanilla JavaScript handling particle canvas animations, active navigation tracking, metric counter animation, project filter tabs, modal dialog handlers, copy-to-clipboard, and toast notifications.

#### [NEW] Assets (`assets/`)
- `adigam_ai.png`: AI-powered adaptive learning assistant interface mockup.
- `foodconnect.png`: Waste-to-welfare food distribution dashboard mockup.
- `simran_avatar.png`: Sleek tech developer avatar.

---

## Verification Plan

### Automated / Browser Verification
1. **Dev Server Execution**: Run a local HTTP dev server in `d:\Portfolio`.
2. **Browser Subagent Testing**:
   - Verify page loading, responsive navbar, and mobile drawer toggle.
   - Test smooth scrolling to all sections: `#about`, `#skills`, `#projects`, `#experience`, `#achievements`, `#contact`.
   - Test metric counter animation when scrolling into the achievements section.
   - Test copy-to-clipboard buttons for email and phone numbers.
   - Test contact form submission and toast notification display.
   - Test opening and closing the interactive resume modal.
   - Inspect console logs for any JavaScript errors or broken links.
3. **Capture Video / Screenshots**: Capture screenshots and recordings verifying the dark-mode aesthetic and flawless design.
