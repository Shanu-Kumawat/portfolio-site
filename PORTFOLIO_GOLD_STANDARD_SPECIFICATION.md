# PORTFOLIO GOLD STANDARD SPECIFICATION

## 1. Purpose & Evaluation Target

This specification defines strict requirements for a developer portfolio website optimized for maximum hiring conversion (interviews/callbacks). It prioritizes recruiter speed, information clarity, and engineering credibility over aesthetics. The goal is to pass the **30-second recruiter scan** and trigger a deeper technical review.

---

## 2. Non-Negotiable Global Constraints

1.  **Speed is Feature #1:** Site must load and be interactive in **<1.5s**. No splash screens, loaders, or "Enter Site" buttons.
2.  **Geography is Mandatory:** Location (City, Country) and Availability (Remote/Hybrid) must be visible in the viewport immediately upon load.
3.  **Zero Friction Navigation:** Standard browser scrolling only. No scroll-jacking, horizontal scrolling primary layouts, or hidden navigation menus.
4.  **Evidence Over Claims:** Show code, live demos, and metrics. Zero tolerance for adjectives (e.g., "Passionate", "Fast learner") or jargon ("Synergy", "Utilize").
5.  **Specialization Wins:** Define a specific role (e.g., "React Developer") rather than a generalist list.
6.  **Work Experience Priority:** If professional experience exists, it must appear **before** personal projects.
7.  **Mobile First:** All content must be fully legible and functional on a **375px** wide viewport.
8.  **Link Integrity:** Every external link must open in a new tab (`target="_blank"`). 0% tolerance for broken links.
9.  **Professional Boundaries:** No gaming links (Steam) or irrelevant socials (Spotify, Instagram) unless directly relevant to a specific built project.

---

## 3. Page-Level Requirements

### Hero Section

*   **Content (Strict Order):**
    1.  **H1 Name:** Full Name.
    2.  **H2 Role:** Specific Job Title (e.g., "Senior Backend Engineer"). NO "slashes" (e.g., "Developer/Designer/Ai Enthusiast").
    3.  **Location:** "Based in [City, Country]" (with icon).
    4.  **Value Prop:** 1 sentence specializing in specific tech stack (e.g., "Specializing in React & Node.js").
    5.  **Actions:** "View Projects" (Anchor scroll) and "Download Resume" (PDF).
    6.  **Socials:** GitHub, LinkedIn, Email (Mailto icon).
*   **Forbidden:** Typing animations, "Hello I am...", vaguely waving hand emojis, carousels.

### About Section

*   **Limit:** Maximum **3 sentences**.
*   **Focus:** Current role, years of experience, core technical focus.
*   **Forbidden:** "Journey" stories, "Since I was a child", motivational quotes.

### Projects Index (Grid)

*   **Layout:** Responsive grid (1 col mobile, 2-3 col desktop).
*   **Sort:** Most impressive/complex project first.
*   **Card Content:**
    *   Thumbnail (High-res 16:9).
    *   Project Title (Functional name, not marketing name).
    *   One-sentence description (What does it do? <15 words).
    *   Tech Stack (Visible text chips/icons, no hover required).
    *   **Buttons:** [Live Demo] and [Source Code].
*   **Requirement:** If a project isn't live or repo is empty, **do not list it**.

### Contact Section

*   **Content:** Email address (visible text linkage to `mailto:`).
*   **Socials:** GitHub, LinkedIn.
*   **Forbidden:** Contact forms (Input fields), "Book a call" widgets.

---

## 4. Project Case Study Template

**Strict Order Required for Top 3 Projects:**

1.  **Project Name:** (Header).
2.  **Problem Statement:** **<15 words** (e.g., "Users needed a way to track crypto without login").
3.  **Role & Constraints:** (e.g., "Solo Developer, 2 weeks").
4.  **What Was Built:** Brief technical summary (2-3 sentences).
5.  **Key Technical Decisions:** Minimum 2 bullet points (e.g., "Chose Next.js for SSR", "Used Redis for caching").
6.  **Trade-offs:** 1 sentence on what could be improved or why a difficult path was chosen.
7.  **Outcome / Impact:** Metrics (Stars, Users, Latency) or completed features.
8.  **Links:** [Live Demo] | [GitHub Repo] | [Documentation].

---

## 5. Design & UX Constraints

*   **Typography:**
    *   Maximum **2** font families.
    *   Sans-serif preferred (Inter, Roboto, System UI).
    *   Minimum font size: 16px (body).
    *   Contrast: WCAG **AAA** compliance (Pure black on white or equivalent).
*   **Colors:**
    *   Maximum **3** colors (Background, Text, One Accent).
    *   Use color *only* to guide attention (buttons, links).
*   **Layout Density:**
    *   Content max-width: **1200px**.
    *   Minimum **60px** whitespace between sections.
    *   Minimum **16px** padding between all elements.
    *   Paragraphs max **80 characters** wide.
*   **Animations:**
    *   Total animations: Maximum **3** across entire site.
    *   Duration: Max **300ms**.
    *   Trigger: Hover/scroll only (No auto-play).
    *   **Banned:** Continuous movement, layout shifting, cursor trails.
*   **Images:**
    *   No blurry thumbnails.
    *   No generic stock photos (Handshakes, Matrix code).

---

## 6. Engineering Credibility Requirements

*   **Pass/Fail Criteria:**
    *   **Repository Quality:** Linked repos must have a `README.md` with setup instructions.
    *   **Live Demo:** Must survive basic load testing (No Heroku spin-up > 5s).
    *   **Performance:** Lighthouse Score > **90** in Performance and Accessibility.
    *   **Technical Depth:** Tech stack chips must be specific (e.g., "PostgreSQL" not just "Database").
    *   **Git Activity:** Link to active GitHub profile.

---

## 7. Forbidden Implementations (Blacklist)

1.  **Skill Bars/Percentages:** No "80% JavaScript" or 5-star ratings.
2.  **Jargon/Buzzwords:** No "Synergy", "Innovative", "Passionate", "Aspiring", "Fast Learner".
3.  **Typing Effects:** No auto-typing headers.
4.  **Scroll Jacking:** No alteration of mouse wheel physics.
5.  **Intro/Splash Screens:** No "Click to Enter" or pre-loaders.
6.  **Audio:** No background music or sound effects.
7.  **Generic "Full Stack":** Do not claim "Full Stack" without backend proofs.
8.  **Contact Forms:** Remove. Use `mailto`.
9.  **Generalist Lists:** Do not list 20+ skills (e.g., including VSCode, Jira). Curate to top 6-8.
10. **Broken/Dead Links:** Immediate failure condition.
11. **Coming Soon:** Do not list incomplete projects.
12. **Theme Toggles:** Deprioritize. Default to system preference.
13. **Gaming/Personal Links:** No Steam, Discord, Spotify widgets.
14. **Carousel/Sliders:** No hiding content behind interaction.
15. **Fake Complexity:** No "Advanced AI" for simple scripts.
16. **Hardcoded Secrets:** Zero tolerance for API keys in code.

---

## 8. Final Validation Checklist

Currently **INCOMPLETE** unless **100%** of checkpoints pass.

*   [ ] **Location Check:** Is "City, Country" visible in the Hero?
*   [ ] **Role Check:** Is the specific Job Title visible in the Hero (No "Aspiring")?
*   [ ] **Speed:** Is Lighthouse Performance Score > 90?
*   [ ] **Links:** Do all external links open in a new tab?
*   [ ] **Links:** Are there zero broken links (404s)?
*   [ ] **Mobile:** Is layout broken on 375px width?
*   [ ] **Resume:** Is there a direct PDF download link?
*   [ ] **Bio:** Is the About section < 3 sentences?
*   [ ] **Skills:** Are all percentage bars/star ratings removed?
*   [ ] **Jargon:** Are words like "Passionate", "Enthusiastic" removed?
*   [ ] **Work Exp:** Is Work Experience listed *before* Personal Projects?
*   [ ] **Contact:** Is the email address visible and copyable?
*   [ ] **Repos:** Do all linked repos have a README?
*   [ ] **Images:** Are all screenshots high-res and aspect-ratio correct?
*   [ ] **Console:** Is the browser console free of errors?
