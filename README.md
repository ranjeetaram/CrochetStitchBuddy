# 🧶 Stitch Buddy: Learn to Crochet

A colorful, interactive beginner crochet app for kids aged 7-15. Kids learn their first project, a small crochet coaster, one stitch at a time. Parents and teachers can see where a child is getting stuck.

The whole app is a single `index.html` file. There is nothing to install and no build step.

## Features

- **Materials checklist:** the basics a beginner needs (hook, yarn, scissors, tapestry needle, stitch markers), with tap-to-check cards.
- **Glossary:** 15 flip-cards covering terms like slip knot, chain, yarn over, single crochet, tension, and frogging, with search.
- **Step tiles:** 8 steps shown as tiles along a "yarn trail." Steps unlock in order, and each has an illustration, instructions, and a tip.
- **Tutorial videos:** embedded beginner videos for the steps where motion is hardest to picture (slip knot, chain, single crochet, turning, fasten off).
- **Hints from Loopy:** three built-in hints per step that cycle each time a child taps the hint button.
- **"I'm Stuck" button:** a low-pressure way for kids to signal difficulty.
- **Progress and badges:** a progress ring and rewards for finishing steps.
- **Gallery:** real projects made by a kid crocheter, for inspiration on what to make next.
- **Parent / teacher dashboard (PIN-protected):** per-step attempts, "stuck" taps, hints used, time spent, and automatic alerts when a step looks tricky, so a parent can reach out to the teacher early.

## Why it exists

Young beginners have to remember unfamiliar terminology, coordinate several hand movements at once, and copy something they just watched. When they get stuck early, it slows their learning and also hurts their confidence and willingness to keep going. This app breaks the project into small steps, explains the vocabulary up front, and surfaces struggle data so adults can step in while the problem is still small.

## Run it

Open `index.html` in any browser, or host it for free on GitHub Pages:

1. Go to **Settings → Pages**.
2. Choose the `main` branch and the root folder, then save.
3. Your app will be live at `https://<your-username>.github.io/<repo-name>/`.

## Known limitations

- **Progress is saved in the browser (localStorage), per device.** The dashboard only shows data from the device being used. A multi-family dashboard with teacher alerts would need a database and logins.
- **The parent PIN (default `1234`) is a soft gate** to keep kids out. It is visible in the page source and is not real security. Change `PARENT_PIN_DEFAULT` in `index.html` to set your own.
- **Gallery photos are embedded in the file,** so anyone who visits the public page can view and save them.
- **Hints are pre-written,** not generated live. Adding AI-generated hints would need a small backend that keeps an API key private.

## Tech

Plain HTML, CSS, and JavaScript. Fonts are loaded from Google Fonts, and tutorial videos are YouTube embeds.

## Credits

Gallery projects were crocheted by the author's daughter. Tutorial videos belong to their original creators and are embedded from YouTube.
