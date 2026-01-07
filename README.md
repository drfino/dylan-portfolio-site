# Dylan Fino - UX Research Portfolio

Built and launched in a day with the help of Copilot AI coding assistant.

## Project Structure

```
dylan-portfolio-site/
├── index.html           # Main portfolio page
├── README.md            # This file
└── assets/
    ├── styles.css       # All styling and responsive breakpoints
    └── images/
        ├── headshot.jpeg         # Profile headshot
        └── [brand logos]         # Client logos (SVG + PNG)
            ├── amazon white.svg
            ├── salesforce.svg
            ├── samsung-galaxy.svg
            ├── xfinity-mobile.svg
            ├── prime.svg
            ├── qualtrics.svg
            ├── figma.svg
            ├── shopify.svg
            ├── comcast.svg
            ├── samsung.svg
            ├── xfinity.svg
            ├── usertesting.svg
            ├── python.svg
            └── chatgpt white.svg
```

## Features

- **Header Section**
  - Circular headshot image
  - Name and role tags (7 total: Senior UX Researcher, Quantitative, Qualitative, etc.)
  - Navigation links (LinkedIn, Resume, Email)
  - Professional bio and research philosophy

- **Brand Carousel**
  - Continuous, seamless loop animation
  - Randomized logo order on page load
  - Pauses on hover
  - Responsive image sizing
  - JavaScript-driven (requestAnimationFrame) for smooth, glitch-free animation

- **Selected Work**
  - **3 Detailed Case Studies:**
    1. Do Off-Amazon Sellers Want Faster Shipping Speeds? (Multi-year roadmap research)
    2. Always-On VOC: AI-Powered Personas (Research infrastructure system)
    3. Why Were Buy with Prime Onboarding Rates So Low? (Rapid usability testing)
  - Expandable `<details>` elements with full research narratives
  - KPI highlights (Outcome, Core Finding, Method)
  - Two-column layouts for readability
  - Methodology tags and project context

- **NPS Joke Section**
  - Interactive 0–10 scale buttons
  - Animated emoji feedback on click
  - Lighthearted engagement element

- **Footer**
  - Auto-updating copyright year
  - LinkedIn and back-to-top links
  - Smooth scroll to top functionality

## Technologies Used

- **HTML5** – Semantic markup, microdata (Schema.org Person)
- **CSS3** – Grid, Flexbox, media queries, animations, object-fit
- **Vanilla JavaScript** – No frameworks required
  - `requestAnimationFrame` for smooth carousel animation
  - Fisher-Yates shuffle for randomizing logo order
  - Event listeners for interactivity (NPS, back-to-top, carousel pause)

## Responsive Breakpoints

The design adapts across three main breakpoints:

- **Mobile** (< 640px) – Single-column layout, stacked navigation
- **Tablet** (640px – 820px) – Adjusted spacing and text sizing
- **Desktop** (820px+) – 3-column header grid (headshot | name/tags | nav)

Images and spacing scale responsively throughout.

## Key Design Decisions

1. **Carousel Animation** – Uses measured `scrollWidth` and `requestAnimationFrame` instead of CSS keyframe duplicates for reliability and smooth looping.

2. **Header Layout** – 3-column CSS Grid at desktop width provides clean visual hierarchy while maintaining full responsiveness.

3. **Expandable Case Studies** – Native HTML `<details>` elements preserve content hierarchy and allow readers to drill deeper on demand.

4. **Brand Logos** – Shuffled on each page load for visual variety; all images optimized with `loading="eager"` and `decoding="async"` to prevent layout shift.

5. **Headshot Positioning** – Uses `object-position: 50% 36%` to frame the face within the circular crop without distortion.

## How to View

### Local Development
1. Clone or download the project
2. Open `index.html` directly in a web browser
   - No build process or dependencies required
   - Serves as a static site

### Deployment
The site can be deployed to any static hosting:
- GitHub Pages
- Netlify
- Vercel
- AWS S3 + CloudFront
- Any standard web server

Simply copy the entire folder structure to your hosting provider.

## Browser Support

Works on all modern browsers supporting:
- CSS Grid and Flexbox
- ES6 JavaScript
- `object-fit` and `object-position`
- `requestAnimationFrame`

## Performance Optimizations

- All images have explicit dimensions (`width` / `height` attributes)
- Brand logos use `loading="eager"` and `decoding="async"` for faster initial render
- CSS uses CSS variables for maintainability and reuse
- Minimal JavaScript; no external dependencies
- Semantic HTML improves SEO and accessibility

## Customization

To adapt this template:

1. **Update Profile Content** – Edit `.summary` paragraphs and `.name` / `.pillrow` in `index.html`
2. **Change Role Tags** – Modify `.pill` spans under the name heading
3. **Add/Remove Case Studies** – Duplicate or remove `.card` articles in the `<main id="work">` section
4. **Update Brand Logos** – Replace images in `assets/images/` and update `src` paths in `.brand-item` divs
5. **Adjust Colors** – Modify CSS variables in `assets/styles.css` (`:root` selector)
6. **Update Links** – Change `href` attributes for LinkedIn, Resume, and Email

## Future Enhancements

Potential additions:
- Dark mode toggle
- Additional case studies or project filtering
- Blog or insights section
- Contact form
- Analytics integration

## License

This portfolio is a personal project. Feel free to use as a template for your own work.

## Contact

- **LinkedIn:** [linkedin.com/in/dylanfino/](https://www.linkedin.com/in/dylanfino/)
