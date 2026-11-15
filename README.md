# Punith Nonavinakere Thandavamurthy — Portfolio Website (v3, terminal edition)

A single-page portfolio built like a terminal. No build step, no dependencies except Google Fonts.

## Files
- `index.html` — the entire site (HTML, CSS, and JS in one file)
- `assets/Punith_Nonavinakere_Thandavamurthy_Resume.pdf` — ATS resume (full name, 2 pages)
- `assets/og-image.png` — 1200x630 social sharing image (terminal-styled)
- `assets/headshot.jpg` — profile photo used in the About section
- `assets/apple-touch-icon.png` — home-screen icon (">_" glyph)

## Run it
Open `index.html` in a browser, or serve the folder:

    python3 -m http.server 8000
    # then visit http://localhost:8000

## Try the terminal
The hero terminal is interactive. Click it and type:
- `help` — list commands
- `about`, `skills`, `contact` — print the info
- `work`, `experience` — jump to those sections
- `resume` — downloads the PDF
- `test` — runs the suites with an ASCII progress bar
- `sudo hire punith` — try it
- Arrow keys browse command history, `clear` wipes the screen

## Host it (free options)
- GitHub Pages: push this folder to a repo, enable Pages on the main branch
- Netlify / Vercel: drag and drop this folder (or the zip) into a new site
- Any static host or S3 bucket works, it is plain HTML
- Note: once hosted, update the og:image / twitter:image paths in index.html to absolute URLs (https://yourdomain/assets/og-image.png) so LinkedIn renders the preview image.

## Design (v3)
- Direction: hand-made terminal/TUI, the opposite of a template. Cream paper canvas, near-black ink, one terminal green. Flat boxes with hard offset shadows, [+] bullets, file-path headers (~/positii-ai/, mphasis/ci-gates.yml), no logo, no gradients, no rounded cards
- Inspired by: OpenCode's block-ASCII wordmark and mono-everything TUI pages, Ghostty's animated ASCII hero, and the interactive terminal portfolios developers ship (working `help` command, neofetch-style info, ASCII banners)
- ASCII animations: the PUNITH block banner decodes from noise on load, a braille spinner runs in the status pill, the test run fills an ASCII progress bar, the stack ticker scrolls, and there is a hand-drawn ASCII test pyramid in Skills
- Motion respects prefers-reduced-motion, content prints cleanly, and everything except the terminal typing works with JavaScript disabled
- Content uses only verified facts from the ATS resume. The Positii-AI visual is captioned as an interface concept shown as a log, not a screenshot
