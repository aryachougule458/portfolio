# Arya Chougule — AI-Powered 3D Personal Portfolio

## Objective
Create a responsive, interactive portfolio that presents the supplied resume as an immersive digital experience while keeping professional information easy to scan.

## Technologies
- React + TypeScript
- Vite
- Three.js with React Three Fiber and Drei
- Framer Motion
- Lucide React icons
- CSS responsive layout and motion-reduction support

## AI tool and prompting approach
AI-assisted development was organized into three prompt iterations: first establish the resume-grounded structure, then improve visual hierarchy and 3D/animation, and finally optimize responsiveness, accessibility, performance, SEO, and maintainability. See `PROMPTS.md`.

## Features
- Full-screen hero with supplied portrait and 3D animated object
- Responsive navigation with active-section indication and mobile menu
- About, project-based experience, projects, skills, education, certifications, and contact sections
- Original resume PDF download (converted from the supplied DOCX for use by the website)
- Smooth anchor navigation, scroll-reveal motion, hover states, and reduced-motion support
- Semantic sections, image alt text, visible interactive controls, SEO title and description
- Resume-based content; no invented employers, roles, metrics, testimonials, or skill ratings

## Installation
Prerequisite: Node.js 18 or newer and npm.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (usually `http://localhost:5173`).

## Production build
```bash
npm run build
npm run preview
```

## Project structure
```text
arya-portfolio/
├── public/
│   ├── arya-profile.jpeg
│   └── Arya_P_Chougule_Resume(1).pdf
├── src/
│   ├── App.tsx
│   ├── main.tsx
│   └── styles.css
├── index.html
├── package.json
├── tsconfig.json
├── vite.config.ts
├── PROMPTS.md
└── README.md
```

## Challenges faced
- Balancing an immersive 3D hero with clear resume readability.
- Presenting projects without adding unverified outcomes or links.
- Keeping the interface usable on smaller screens and for visitors who prefer reduced motion.

## Improvements made
- Used responsive breakpoints to simplify the visual composition on mobile.
- Reduced canvas pixel ratio to control rendering cost.
- Added reduced-motion CSS and Framer Motion handling.
- Added descriptive metadata, semantic landmarks, keyboard-accessible links/buttons, and alt text.

## Future scope
- Add verified project repository/demo URLs when available.
- Add automated accessibility and cross-device testing.
- Optimize portrait assets further and measure performance with Lighthouse.
- Add project screenshots only when actual screenshots are available.

## Notes before submission
1. The provided resume was a DOCX, not a PDF. A PDF copy was generated from that supplied document and placed in `public/` so the website's Download Resume button works.
2. The provided photograph is used as the portfolio portrait.
3. The assignment requests screenshots of each section and a mobile view. Capture these after running the site locally at desktop and mobile widths; screenshots are not fabricated in this source package.
4. No employer or formal job role was added because none was listed in the resume. The Experience section transparently describes project-based work.
