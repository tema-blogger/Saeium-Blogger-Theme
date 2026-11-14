# Saeium 1.5.0 verification

Date: 14 November 2026. Live site: [saeium.blogspot.com](https://saeium.blogspot.com/).

## Reference audit

The live Medium homepage used a 24px/30px bold Sohne story title. A live Medium article used a 42px/52px bold Sohne headline and 20px/32px Source Serif Pro body text. Sohne is proprietary, so Saeium uses Inter for a similar sans-serif hierarchy and Source Serif Pro for reading text. The Saeium wordmark remains Georgia.

## Follow behavior

The theme builds the official Blogger follow URL from `data:blog.blogId`. On the live demo, each Follow blog link resolves to `https://www.blogger.com/followers/follow/8516721557191257277`. The destination displayed the correct blog's follow confirmation. No follow was submitted during verification. Blogger states that followed blogs appear in the follower's Reading List. This is not an email newsletter.

Follow blog appears in the desktop header, left rail, mobile drawer, article byline, publication card, sidebar, and footer. The native Followers iframe was removed after it rendered an empty panel; the direct follow links remain functional.

## Live checks

| Check | Result |
| --- | --- |
| Blogger theme editor | Accepted v1.5.0 with “Update berhasil.” |
| XML and JavaScript | Builder and validator passed; embedded JavaScript passed `node --check` |
| Original gadgets | Eight original sections and nine widgets retained |
| Desktop article headline | Inter, 42px, 52.08px line height, weight 700 |
| Article body | Source Serif Pro, 20px, 32px line height |
| 390px mobile article headline | Inter, 36px |
| 390px mobile home card title | Inter, 24px |
| Web font loading | `document.fonts.check` true for Inter and Source Serif Pro |
| Horizontal overflow | None on live desktop or 390px mobile views |
| RSS links | No visible RSS link in the navigation or footer |

Desktop article and mobile drawer captures were taken from the live site after the update. Earlier preview files were removed from the current repository during the v1.6.1 cleanup.

## Limits

The Follow blog action depends on a visitor confirming in Blogger while signed in. Google Fonts also requires a network request; fallback fonts are defined for failed requests. Existing comment permissions are controlled by the blog's Blogger settings.
