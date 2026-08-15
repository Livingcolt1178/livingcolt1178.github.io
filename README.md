# Livingcolt1178.github.io

Personal portfolio site. Plain HTML and one stylesheet, no build step.

Live at **https://livingcolt1178.github.io**

## Deploying

1. Create a repository named exactly `Livingcolt1178.github.io` on GitHub.
2. Copy the contents of this `site/` folder into the repository root, so that
   `index.html` sits at the top level (not inside a `site/` subfolder).
3. Commit and push to `main`.
4. In the repository, go to **Settings → Pages**, set Source to
   **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
5. The site is live in a minute or two. Pushing to `main` redeploys it.

## Files

| File | Page |
| --- | --- |
| `index.html` | Home |
| `about.html` | About |
| `career-goals.html` | Career goals |
| `resume.html` | Resume |
| `portfolio.html` | Portfolio index |
| `contact.html` | Contact |
| `riscv-cpu.html` | RISC-V CPU project |
| `digital-signal-processing.html` | Rolling Average Filter project |
| `uart-core.html` | UART core project |
| `fsm-lock.html` | FSM lock project |
| `ai-code-comparison.html` | AP Research paper |
| `404.html` | Not-found page, served automatically by GitHub Pages |
| `style.css` | Shared stylesheet |
| `assets/` | Figures, diagrams, PDFs |

## Before you go live

**Three files still need to be added to `assets/`:**

- `nicholas-bramhall-ece-resume-2026.pdf` — linked from `resume.html`
- `degree-plan.pdf` — linked from `career-goals.html`
- Nothing else is required, but three photo placeholders are waiting for images:
  the Spartan Edge board (`riscv-cpu.html`), the DSP bench (`digital-signal-processing.html`),
  and the Basys3 with the unlock LED lit (`fsm-lock.html`). Each is a
  `<div class="nb-slot">` — replace it with an `<img src="assets/your-photo.jpg" alt="...">`.

**Images still hosted on Weebly.** The code screenshots on the DSP page and the
photos on Home and About load from `nicholasbramhall.weebly.com/uploads/...`. They
work while that site is up. Before taking Weebly down, download each one into
`assets/` and update the `src` attributes, or those figures will break. Search the
HTML for `weebly.com/uploads` to find all of them.

**The contact form** posts to Formspree. Create a free form at formspree.io and
replace `YOUR_FORM_ID` in `contact.html`, or delete the form and keep the email
address. GitHub Pages serves static files only and cannot process a POST itself.

## Editing

Every page is a standalone HTML file with inline styles for layout and a shared
`style.css` for resets, navigation, and responsive rules. There is no framework
and nothing to compile — edit the HTML directly and push.

Design rules for the site (colors, type scale, component patterns) are documented
in `theme.md` in the design project this site was built from.
