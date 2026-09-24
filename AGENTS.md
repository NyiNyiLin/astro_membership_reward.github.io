# AGENTS.md

## Project purpose

This repository contains a GitHub Pages website that presents membership reward program details. The site should make it easy for visitors to understand membership levels, benefits, points, eligibility, redemption rules, expiration policies, and frequently asked questions.

## Technical constraints

- Build a static website that works on GitHub Pages.
- Use HTML5, CSS, and vanilla JavaScript only unless the user explicitly requests a different GitHub Pages-compatible approach.
- Do not add server-side code, databases, private environment variables, or APIs that require secrets.
- Do not depend on Node.js, a build step, or a package manager unless explicitly requested.
- Use relative URLs for internal pages and assets so the site works from a GitHub project subpath.
- Keep the main entry point at `index.html`.
- Put reusable styles in `assets/css/` and scripts in `assets/js/` when the site grows beyond a small single-file page.
- Store images and icons locally under `assets/` when practical. Do not rely on fragile hotlinks.

## Design and content goals

- Prioritize clear membership reward information over decorative effects.
- Use an inviting, trustworthy visual style suitable for a loyalty or rewards program.
- Present important information in scannable sections such as:
  - program overview;
  - membership tiers and qualification requirements;
  - benefits by tier;
  - how to earn and redeem points;
  - point value, validity, and expiration;
  - terms, limitations, and exclusions;
  - frequently asked questions;
  - contact or support information.
- Use cards, comparison tables, badges, and concise calls to action only when they improve understanding.
- Never invent reward rates, prices, dates, legal terms, or contact details. Use clearly marked placeholders when source content has not been provided.

## Responsive behavior

- Design mobile-first and support screens from 320px wide upward.
- Add the viewport meta tag to every page.
- Avoid fixed-width layouts and horizontal page scrolling.
- Use flexible grids, wrapping layouts, responsive spacing, and fluid media.
- Convert wide tier comparison tables into a mobile-friendly layout, such as stacked cards or a horizontally scrollable region with a visible label.
- Ensure navigation, buttons, and interactive controls remain easy to use by touch.
- Use touch targets of approximately 44 by 44 CSS pixels or larger.
- Test at common mobile, tablet, and desktop widths.

## Accessibility

- Use semantic HTML with a logical heading hierarchy and landmark elements.
- Provide a visible keyboard focus state for every interactive element.
- Ensure all functionality works with a keyboard.
- Associate form controls with labels and provide useful alternative text for meaningful images.
- Maintain readable font sizes, line heights, and sufficient color contrast.
- Do not communicate membership status or eligibility with color alone.
- Respect `prefers-reduced-motion` and keep animation optional and subtle.

## Performance and compatibility

- Keep the page lightweight and fast on mobile connections.
- Prefer system fonts or locally hosted optimized fonts.
- Optimize images and specify their dimensions to reduce layout shift.
- Defer non-critical JavaScript and avoid blocking third-party scripts.
- Use progressive enhancement: core reward information must remain readable if JavaScript is unavailable.
- Support current versions of major mobile and desktop browsers.

## SEO and sharing

- Give every page a descriptive title and meta description.
- Include appropriate Open Graph metadata when final branding and share imagery are available.
- Use descriptive link text and human-readable page structure.
- If multiple pages are added, keep navigation consistent and ensure every page is reachable through normal links.

## Implementation conventions

- Keep HTML, CSS, and JavaScript readable and organized.
- Use CSS custom properties for shared colors, spacing, typography, and radii.
- Prefer reusable classes over repeated inline styles.
- Use JavaScript only for behavior; do not render essential content exclusively with JavaScript.
- Avoid large frameworks and dependencies for features that can be implemented simply with platform APIs.
- Add comments only where they explain a non-obvious decision.
- Preserve existing user content and unrelated changes.

## Verification checklist

Before considering a change complete:

1. Open the site from the repository root and confirm all pages, links, images, and assets load with relative paths.
2. Check the layout at approximately 320px, 375px, 768px, 1024px, and 1440px widths.
3. Confirm there is no unintended horizontal scrolling.
4. Navigate all controls using only the keyboard and verify visible focus states.
5. Check headings, landmarks, labels, alternative text, and color contrast.
6. Confirm essential membership information is available without JavaScript.
7. Check the browser console for errors.
8. Validate that the result can be hosted as a static GitHub Pages site without a server-side runtime.
