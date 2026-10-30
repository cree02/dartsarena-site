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

## Promo video
`assets/video/dartsarena-promo.mp4` is an H.264 copy (made with `avconvert
-p Preset1920x1080`) of the original HEVC `.mov` in `assets/Videos/`, which is
git-ignored because Firefox and many Windows browsers can't play HEVC. The
poster is the frame at 0.6 s. The video autoplays muted only while on screen.

## App Store link
One listing for Mac and iOS (universal purchase): https://apps.apple.com/app/id6820357271
Mac went live first. Badges are Apple's official SVGs from
toolbox.marketingtools.apple.com (`assets/badge-mac-app-store.svg`, and
`assets/badge-app-store.svg` ready for iOS).

When iOS is approved, in `index.html` (search `iOS LAUNCH`): swap both badges
to `badge-app-store.svg` / "Download on the App Store", remove "iPhone & iPad
version coming soon" from the hero note, and reword the bottom "out now for
Mac" line. The link stays the same.

## Policy changes
The privacy text must match the App Store privacy answers
(`../DartsArena/AppStore/app-privacy.md`). Update the "Last updated" date
when it changes.
