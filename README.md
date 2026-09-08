# GCS12th — College & Career Readiness activities

Interactive lessons for **College & Career Readiness**, Grade 12.
Mr. Babb · Paul Public Charter School · 2026–2027

**Live site:** https://babbm19-alt.github.io/GCS12th/

The capitalisation matters — `GCS12th`, not `gcs12th`. GitHub Pages URLs are
case-sensitive.

---

## Turn the site on (one time, ~1 minute)

1. **Settings** → **Pages** (left sidebar)
2. **Source:** Deploy from a branch
3. **Branch:** `main`  ·  **Folder:** `/ (root)`
4. **Save**, then wait about a minute

Then load **the site root** and confirm both lesson cards are on it. Checking a
lesson URL alone is not enough — a stale `index.html` still serves the old hub
while the new lesson pages resolve fine, which is exactly how the last repo went
quietly wrong.

---

## What students open

| Lesson | Link |
|---|---|
| Hub | https://babbm19-alt.github.io/GCS12th/ |
| CCR 1.1.1 — Letter to Your Future Self | https://babbm19-alt.github.io/GCS12th/ccr-111-letter-to-future-self.html |
| CCR 1.1.2 — Values, Identity & Fit | https://babbm19-alt.github.io/GCS12th/ccr-112-values-and-college-fit.html |

Plain URLs. No login, no Claude account, no download. They work on a Chromebook,
on a phone, and offline once the page has loaded.

---

## Files

```
index.html                              the hub students land on
ccr-111-letter-to-future-self.html      CCR 1.1.1
ccr-112-values-and-college-fit.html     CCR 1.1.2
.nojekyll                               tells Pages to serve the files as-is
README.md                               this file
```

Every page is **one self-contained file** — no stylesheet, no scripts, no images,
no build step. That is deliberate: a lesson keeps working if it is emailed,
downloaded, or opened with no network.

---

## Adding the next lesson

1. Name it `ccr-<unit><lesson>-<slug>.html`, all lowercase, hyphens, no spaces.
2. Upload it to the repo root.
3. Add one `.item` card to the grid in `index.html`, in teaching order.
4. Load the site root and confirm the card is there.

### The upload trap — read this before dragging files in

If a file with the same name is already in your Downloads folder, the browser
saves the new one as `name_2.html` and **that** is what lands in the repo. The
hub then links to a file that does not exist.

Before uploading: clear the old copies out of Downloads, or unzip into a fresh
empty folder. After uploading, check the file list — every name should be exactly
as listed above, with no `_2`, no ` 2`, no `(1)`.

---

## What is deliberately NOT here

**Lesson plans and answer keys.** This repo is public and students can read
anything in it. The teacher lesson plans, the weekly plans, and the options
spreadsheet stay off the site.

The answers inside the lesson pages are stored as salted hashes rather than plain
text, so viewing source does not reveal them. That defeats a curious student, not
a determined one with a browser console — treat the exit tickets as formative.
