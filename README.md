# Zaleene Brand Site

Single-page personal brand website for Zaleene, built with plain HTML and CSS.

No framework, no build process, no runtime dependencies.

## Project Structure

- `index.html`: complete page markup, content, and small client-side form script.
- `styles.css`: full design system and responsive styling.
- `images/`: visual references and hero image assets.
	- `stylist01.jpg` is used as the hero mood image.
- `CNAME`: GitHub Pages custom domain configuration (`zalien.me`).

## Current Live Setup

- Repository: `dreadstache/stylist-brand-site`
- Branch for deployment: `master`
- Hosting: GitHub Pages
- Custom domain: `zalien.me`
- Also supported: `www.zalien.me` (CNAME to GitHub Pages)

## Design Direction

The current aesthetic is a warm editorial palette built from the provided visual references:

- Plum / burgundy / wine tones
- Deep teal accents
- Antique gold highlights
- Antique ivory typography on dark sections
- Slightly warm, antique-beige paper background for light surfaces

## Navigation UX

- Hero section: single "Next" down-arrow control
- Middle sections: subtle up/down navigation controls with "Next" label
- Final section: single "Back to top" control

## Contact Form Behavior

The form submits through FormSubmit (no backend required in this repo):

- Endpoint: `https://formsubmit.co/invaderzalien@icloud.com`
- Dynamic subject format: `New Website Contact - {Sender Name}`
- Includes a loading state (`Sending...`) on submit
- Redirects back with `?sent=1#connect` and shows a "Message sent" confirmation

Important:

- FormSubmit requires one-time email activation for the target address.

## Local Preview

1. Open `index.html` directly in a browser for quick visual checks.
2. For best behavior parity with hosted mode, use a lightweight local server if desired.

## Deploy / Update Workflow

1. Commit and push changes to `master`.
2. GitHub Pages auto-builds from repository root.
3. If Pages queue appears stale, manually trigger a build:
	 - `gh api -X POST repos/dreadstache/stylist-brand-site/pages/builds`

## Domain and DNS Notes

For `zalien.me` + `www.zalien.me` on GitHub Pages:

- Apex `A` records:
	- `185.199.108.153`
	- `185.199.109.153`
	- `185.199.110.153`
	- `185.199.111.153`
- `www` CNAME:
	- `dreadstache.github.io`

After DNS propagation:

1. Confirm GitHub Pages domain verification.
2. Enable **Enforce HTTPS** in GitHub Pages settings when available.

## Editing Notes

- Keep files ASCII unless a character is intentionally needed.
- Preserve the current responsive behavior and section semantics.
- When adjusting colors, update root variables first in `styles.css` to maintain consistency.
