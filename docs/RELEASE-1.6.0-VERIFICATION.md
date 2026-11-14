# Saeium v1.6.0 verification

Date: 2026-11-15. Live demo: <https://saeium.blogspot.com/>.

## Image diagnosis and fix

The earlier Keep reading cards showed abstract placeholders because the summary feed had no `media$thumbnail` for any of the six demo posts. Their first images were present in full post content. The new article recommendation loader reads `/feeds/posts/default`, extracts the first safe HTTP(S) image when needed, and requests appropriately sized images. It retains the placeholder for genuinely imageless posts.

The live article `a-walk-without-destination.html` showed four loaded photo covers after setting `relatedCount=4` in Layout. The covers link to their posts. [Live screenshot](../preview-related-v1.6.0.png).

## Configuration and preservation

- The uploaded XML passed XML parsing and JavaScript syntax checks.
- The original eleven gadget IDs and stored gadget settings matched the v1.5.1 live baseline.
- The live Layout panel showed twelve named sections and fourteen gadgets. The Theme settings, Explore links, and Footer shortcuts edit forms opened; the Theme settings value was saved live.
- The article displayed a reading progress bar, and the live count setting produced four related cards.
- The public navigation and footer rendered the extra links.

## Responsive check

At a 390px emulated viewport, the homepage and article had `clientWidth=390` and `scrollWidth=390`; no horizontal overflow was observed. The hamburger opened the menu with `aria-expanded=true`, and four related images remained in the article.

## Speed checks and changes

The homepage's requested native thumbnails were reduced from 400px to 240px. Related article images request up to 640px and use lazy loading. Each of the six demo posts has a hidden first source image used for cover metadata; these were marked `loading="lazy" decoding="async"`. On the checked live article, the browser requested the visible Blogger-proxied hero image and did not request the hidden 1600px Unsplash source image.

One desktop Chrome navigation with cache disabled after deployment produced these **observations**, not a benchmark score:

| Page | TTFB | DOM interactive | FCP | LCP | Load | CLS |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Home | 339 ms | 1,224 ms | 1,164 ms | 1,412 ms | 1,307 ms | 0 |
| Article | 226 ms | 1,392 ms | 1,288 ms | 1,404 ms | 2,900 ms | 0 |

The PageSpeed Insights API returned HTTP 429, so no PageSpeed or Lighthouse score is claimed. Earlier single-run timings used a different cache state and are not directly comparable. Network, device, fonts, and Blogger response times can change these values.

## Limits

Related photos depend on each post having an image and on the public post feed being available. The settings gadget controls the listed appearance and behavior options; it does not expose every CSS declaration or Blogger internal option. Saved stories and comment Likes are local to a visitor's browser.
