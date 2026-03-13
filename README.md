[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/8NpkA7e4)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23117179&assignment_repo_type=AssignmentRepo)
# Assignment 1: Responsive Portfolio Website

**Course:** CSC4035 Web Programming and Technologies
**Weight:** 5% of final grade
**Due:** Week 6, Friday 11:59 PM

---

## Overview

Create a professional, responsive portfolio website showcasing your skills, projects, and contact information. This assignment assesses your HTML5 and CSS3 skills, including semantic markup, modern layout techniques (Flexbox/Grid), and responsive design principles.

**Important:** No CSS frameworks (Bootstrap, Tailwind, etc.) are allowed. All CSS must be hand-written.

---

## Requirements

### Functional Requirements

Your portfolio must include **4 or more sections**:

| Section | Required Content |
|---------|------------------|
| **Home/Hero** | Your name, tagline, and call-to-action button |
| **About** | Professional bio (150+ words), profile image, skills list |
| **Projects** | Minimum 3 project cards with title, description, image, and links |
| **Contact** | Contact form with validation attributes (name, email, message) |

### Technical Requirements

| Requirement | Description |
|-------------|-------------|
| **HTML5** | Valid semantic HTML (header, nav, main, section, article, footer) |
| **CSS3** | External stylesheet only (no inline styles) |
| **CSS Variables** | Use custom properties for colors and spacing |
| **Flexbox** | Use for at least one layout component |
| **CSS Grid** | Use for at least one layout component |
| **Responsive** | Mobile-first with minimum 3 breakpoints |
| **Accessibility** | Alt text, form labels, color contrast, heading hierarchy |

### Breakpoints Required

```css
/* Mobile-first base styles */

/* Tablet (768px and up) */
@media (min-width: 768px) { }

/* Desktop (1024px and up) */
@media (min-width: 1024px) { }

/* Large Desktop (1200px and up) - optional */
@media (min-width: 1200px) { }
```

---

## Project Structure

```
csc4035-assignment1-portfolio/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # Main stylesheet
├── images/             # Your images (profile, projects, etc.)
├── screenshots/        # Screenshots at different breakpoints
│   ├── mobile.png
│   ├── tablet.png
│   └── desktop.png
└── README.md           # This file (update with your info)
```

---

## Getting Started

1. **Clone this repository** to your local machine
2. **Open `index.html`** in your code editor
3. **Complete the TODO comments** in each file
4. **Test responsiveness** using browser developer tools
5. **Take screenshots** at mobile, tablet, and desktop sizes
6. **Commit and push** your changes regularly

---

## Grading Rubric (100 points)

| Criterion | Points | Description |
|-----------|--------|-------------|
| **HTML Structure & Semantics** | 20 | Valid HTML5, semantic elements, proper document structure |
| **CSS Styling & Design** | 20 | Professional design, cohesive color scheme, typography |
| **Flexbox & Grid Usage** | 20 | Both techniques used appropriately and effectively |
| **Responsive Design** | 20 | Mobile-first, 3+ breakpoints, no horizontal scrolling |
| **Content & Completeness** | 10 | All sections complete with quality content |
| **Code Quality** | 10 | Clean, organized, well-commented code |

### Automated Tests (40% of grade)

The following are checked automatically on each push:
- HTML validation (no errors)
- Required HTML elements present
- CSS file linked correctly
- Required sections exist
- Responsive meta tag present

---

## Submission Checklist

Before submitting, verify:

- [ ] All 4 sections are complete (Home, About, Projects, Contact)
- [ ] HTML validates with no errors
- [ ] CSS uses custom properties (variables)
- [ ] Flexbox is used for at least one component
- [ ] CSS Grid is used for at least one component
- [ ] Site is responsive at all breakpoints
- [ ] All images have alt text
- [ ] Form inputs have labels
- [ ] Screenshots added to `/screenshots` folder
- [ ] README updated with your information

---

## Your Information

**Name:** Samuel Chibinji Mwanza
**Student ID:** 2021465934
**Design Theme:** Professional grey and blue color scheme with clean, modern aesthetics suitable for a tech portfolio

### CSS Techniques Used
CSS Custom Properties - For colors, spacing, typography, and transitions

Flexbox - Used in navigation, hero section, footer, skills list, and project card links

CSS Grid - Used in about section (2-column layout on tablet/desktop) and projects grid (1-2-3 columns responsive)

Media Queries - Breakpoints at 480px, 768px, 1024px, and 1200px

CSS Animations - Fade-in effects on hero section, staggered animations on project cards and skills

CSS Transitions - Hover effects on buttons, cards, and navigation links

CSS-only Hamburger Menu - Using checkbox hack (no JavaScript)

Print Stylesheet - Optimized for printing with hidden navigation and interactive elements

Dark Mode Support - CSS variables ready for dark mode toggle

Accessibility Features - Focus indicators, skip-to-content link, reduced motion support, high contrast mode

### Challenges & Solutions
Challenge 1: Creating a responsive navigation that works well on all devices
Solution: Implemented a mobile-first approach with a CSS-only hamburger menu using the checkbox hack. The navigation transforms from a hidden hamburger menu on mobile to a horizontal navigation bar on desktop, all without JavaScript.

Challenge 2: Ensuring the bio section meets the 150+ word requirement while maintaining readability
Solution: Structured the bio with four clear paragraphs covering background, interests, motivation, and unique perspective. Each paragraph flows naturally into the next, creating a compelling narrative about my journey as a Zambian software engineer.

Challenge 3: Making project cards maintain consistent height with varying content
Solution: Used CSS Grid for the project container to ensure equal height rows, and Flexbox within each card (display: flex; flex-direction: column;) to push the links to the bottom regardless of description length.

Challenge 4: Implementing a professional color scheme that's both modern and accessible
Solution: Chose a sophisticated grey and blue palette with sufficient contrast ratios (meeting WCAG guidelines). Used CSS variables throughout for easy maintenance and future dark mode implementation.

Challenge 5: Creating smooth animations without impacting performance
Solution: Used CSS transforms and opacity for animations (which are GPU-accelerated) instead of properties like left or top. Implemented prefers-reduced-motion media query to respect user accessibility preferences.

### Credits
Images
All images used in this portfolio are either personal photographs or screenshots of my own projects:

profile.jpg – Personal photograph taken at University of Zambia campus

pharmacy-pos.jpg – Original screenshot of Pharmacy Point of Sale System 

zamprep.jpg – Original screenshot of a parent using the zamprep app with their child

unza.jpeg – Photograph of University of Zambia campus. Own work taken at the Great East Road campus, Lusaka.

Fonts
No external fonts or font services (Google Fonts, Adobe Fonts, etc.) were used in this project. The site uses the native system font stack for optimal performance, cross-platform consistency, and readability:

Resources
The following documentation and online resources were consulted during development to ensure best practices and proper implementation:

Mozilla Developer Network (MDN)

HTML documentation for semantic structure and element usage

CSS reference for properties, values, and browser support

CSS Grid Layout guide for implementing responsive project cards

Flexbox guide for navigation and footer layouts

Accessibility guides for ARIA labels and focus management

CSS-Tricks

"A Complete Guide to Grid" – Referenced for advanced grid techniques and responsive breakpoints

"A Complete Guide to Flexbox" – Used for understanding flex container and item properties

"The Checkbox Hack" – Provided the foundation for the CSS-only hamburger menu implementation

Web Accessibility Resources

W3C Web Accessibility Initiative (WAI) – Guidelines for semantic HTML and keyboard navigation

WebAIM – Contrast checking and accessibility best practices

A11Y Project – Focus management and skip navigation links

Validation Tools

W3C HTML Validator – Used to ensure markup is error-free

W3C CSS Validator – Used to validate all CSS properties and values

WAVE Web Accessibility Tool – Used to verify accessibility compliance

---

## Academic Integrity

- All code must be your own work
- No CSS frameworks or libraries allowed
- Images must be royalty-free or your own (credit sources)
- Plagiarism detection tools will be used

**Violations result in zero marks and academic misconduct reporting.**

---

## Extension Opportunities (Bonus: up to +10%)

- Dark/light mode toggle with CSS (+3%)
- CSS animations/transitions (+3%)
- CSS-only hamburger menu (+2%)
- Print stylesheet (+2%)
