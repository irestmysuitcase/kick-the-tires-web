# Landing Page Redesign Task

## Reference
Look at https://www.grammarly.com for design inspiration. We want a similar level of polish and confidence — clean, spacious, professional, trustworthy.

## Color Scheme
Primary brand color: warm yellow (#FBBC04 or similar golden yellow)
Use this yellow for:
- Primary CTA button ("Add to Chrome — It's Free")
- Section accent labels (the "FREE CHROME EXTENSION", "HOW IT WORKS" etc.)
- Hover states and highlights

Supporting colors:
- Slate-900 (#0f172a) for headings and primary text
- Slate-600 (#475569) for body text
- Slate-100 (#f1f5f9) for alternating section backgrounds
- White (#ffffff) for main background
- The extension's existing verdict colors for inline mentions: emerald for "Recommended", amber/yellow for "Caution", red for "Avoid"

## Design Direction (Grammarly-inspired)
- **Hero**: Center-aligned, large headline, generous vertical padding (py-32 or more). The headline should feel bold and confident. Keep the tagline "The marketplace works for dealers. This works for you." with "This works for you." in the brand yellow color.
- **Typography**: Keep DM Sans but make the hero headline larger (text-5xl md:text-6xl). Consider making the tagline line slightly italic or using a serif font for just the hero headline for contrast (like Grammarly uses).
- **CTA button**: Yellow (#FBBC04) background with dark text, rounded-full (pill shape like Grammarly), generous padding. Add a subtle shadow.
- **Spacing**: Much more generous whitespace between sections than current. Let things breathe.
- **Feature cards**: Clean white cards with subtle border/shadow on the light grey section background. The screenshot placeholders should have rounded corners and a subtle shadow.
- **Supported models section**: Keep the grid but make the cards slightly more refined — perhaps just text on white with a subtle left border accent in yellow.
- **Footer**: Simple, light, understated.
- **Nav**: Minimal — logo + "Privacy" link. No hamburger menu needed (only 2 pages).

## Logo
Use the 🛞 emoji followed by "Kick the Tires" in the nav. The emoji appears in both index.astro and privacy.astro nav sections.

## Pages to Update
1. `src/layouts/Layout.astro` — update body classes for light theme
2. `src/pages/index.astro` — full homepage redesign
3. `src/pages/privacy.astro` — match new styling (keep all privacy policy content identical, just update visual styling)

## Content (do NOT change the copy)
Keep all text content exactly as it is. Only change styling, colors, spacing, and layout. The privacy policy text must remain word-for-word identical.

## Tech Stack
- Astro 6 with Tailwind CSS v4 (via @tailwindcss/vite plugin)
- Tailwind is imported via `@import "tailwindcss";` in `src/styles/global.css`
- Google Fonts: DM Sans + DM Mono (loaded in Layout.astro)
- No JavaScript needed — pure static HTML/CSS

## Screenshot Placeholders
Keep the screenshot placeholder divs but style them as polished empty states:
- Light grey background with rounded-xl corners
- Subtle shadow
- Placeholder text centered inside
- aspect-video ratio maintained
