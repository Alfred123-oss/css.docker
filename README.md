
Alfred's Poultry Farm - Kiambu
(HTML5 + CSS3 Practical Project with Docker)
Overview
This project demonstrates a styled HTML5 + CSS3 website for Alfred's Poultry Farm in Kiambu.
It highlights:
    Semantic HTML5 structure
    Accessibility best practices (skip links, alt text, focus indicators)
    Responsive design with modern CSS3 (Flexbox, Grid, variables, dark mode)
	Media embedding (images, audio, video with captions)
	Packaged and served using Docker (nginx:alpine)
Structure
	index.html → Home page (semantic layout, skip link, micro-elements, cards).
	about.html → About the farm (history, mission, values, lists).
	media.html → Farm images, audio, video with captions.
	extras.html → Tables, quotes, and interactive elements (details/summary, blockquotes).
Assets
	CSS → assets/css/styles.css (custom styling, responsive, dark mode).
	Images → stored in assets/images/
	Audio → stored in assets/audio/
	Videos → stored in assets/video/
	Captions → stored in assets/captions/
Styling (CSS3 Features)
	Design tokens: CSS variables for colors, typography, spacing.
	Dark mode: Uses prefers-color-scheme media query.
	Layout: Flexbox for nav/header/footer; Grid for main content and sidebars.
	Typography: System font stack + modular type scale.
	Components:
	.card component (padding, shadow, border-radius).
	Styled tables with striped rows (:nth-child).
	Responsive media (max-width: 100%).
	Utilities: Custom classes (.mt-2, .mb-3, .text-center, .visually-hidden).
	Accessibility & motion:
	Focus indicators for all links and buttons.
	Reduced motion handling with prefers-reduced-motion.
Design Decisions
Palette (CSS Variables):
	--bg: light background (#fdfdfd), #111 in dark mode.
	--fg: dark foreground text (#222), #eee in dark mode.
	--brand: green (#3a7d44) to reflect farming/nature theme.
	--brand-contrast: white (#fff) for contrast text.
	--muted: gray (#666) for captions and secondary text.
Typography System:
	Base font: system stack (-apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif).
	Scale:
	--h1: 2rem
	--h2: 1.5rem
	--body: 1rem
	Line height: 1.6 for readability.
Spacing Scale (CSS Variables):
	--space-1: 0.25rem
	--space-2: 0.5rem
	--space-3: 1rem
	--space-4: 1.5rem
	--space-5: 2rem
Components:
	Cards: applied on the home page to highlight farm sections.
	Tables: striped design with hover effect for readability.
	Media: responsive containers with subtle captions.
Accessibility:
	All text passes WCAG AA contrast.
	Skip link styled to appear on focus.
	Clear focus states with visible outlines.
	Motion respects prefers-reduced-motion.
