# playdartsarena.com

Marketing site for the DartsArena app: plain static HTML/CSS, no build step.
Hosted on GitHub Pages with the custom domain in `CNAME`.

| URL | File | Used for |
|---|---|---|
| `/` | `index.html` | Marketing URL in App Store Connect |
| `/support/` | `support/index.html` | Support URL (required) |
| `/privacy/` | `privacy/index.html` | Privacy Policy URL (required) |
| `/support.html`, `/privacy-policy.html` | redirects | old file names |

Images in `assets/` are web-sized copies of `../DartsArena/AppStore/screenshots`
and `../DartsArena/Design/app-icon-source.jpg` (made with `sips`).

## At launch
In `index.html`, replace the "Coming soon" span (search for `LAUNCH:`) with a
link to the App Store page, and change "coming soon" in the bottom section.

## Policy changes
The privacy text must match the App Store privacy answers
(`../DartsArena/AppStore/app-privacy.md`). Update the "Last updated" date
when it changes.
