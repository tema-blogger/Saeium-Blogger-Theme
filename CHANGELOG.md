# Changelog

## 1.6.0 — 2026-11-15

- Fixed empty related-story covers by reading each post's first image from the full Blogger feed when no feed thumbnail exists. Related cards now use 640px images, load lazily, link from the cover, and prioritize shared topics.
- Added a compact article reading progress bar and a native Theme settings gadget for colors, font presets, reading width, article text sizes, related-story count and visibility, progress visibility, follow label, and common section headings.
- Added native Link List gadgets for extra navigation and footer shortcuts; link names, destinations, and order can be edited in Layout.
- Reduced home thumbnail requests from 400px to 240px. Marked the hidden source image in all six demo articles as lazy to avoid a duplicate 1600px download while keeping the visible Blogger-proxied cover.
- Verified the live 390px home and article layouts without horizontal overflow, the three new gadget edit forms, four related images after setting `relatedCount=4`, and browser paint metrics. PageSpeed Insights API returned HTTP 429, so no PageSpeed score is claimed.
- Preserved the eleven existing gadget IDs and settings. The live theme now has twelve sections and fourteen widgets. Updated the English documentation and GitHub repository.

## 1.5.1 — 2026-11-14

- Added a Saeium v1.5.1 label and clearer Indonesian section names to the live Blogger Layout panel.
- Grouped the main content and sidebar without nested panel frames and removed stray list markers from layout mode.
- Added native HTML/JavaScript gadgets for sidebar follow copy and footer description, while keeping the official follow URL and the existing public wording as defaults.
- Preserved all eight original sections, nine original widgets, and their stored settings; the live panel now has nine sections and eleven widgets.
- Verified both new gadget edit forms, the live homepage, and an article. GitHub was not updated.

## 1.5.0 — 2026-11-14

- Added official Blogger Follow blog links to the desktop header, left navigation, mobile drawer, article byline and publication card, sidebar, and footer.
- Used Inter for interface text and headlines and Source Serif Pro for article reading text, with fallback fonts. Adjusted the article headline and body sizes to match the audited Medium hierarchy.
- Removed an empty native Followers iframe from the sidebar while retaining the working follow action.
- Verified the live desktop and 390px mobile home/article layouts, loaded fonts, follow destination, and lack of horizontal overflow.
- Preserved all eight original Blogger sections and nine widgets. No GitHub repository was updated.

## 1.4.1 — 2026-11-14

- Aligned the desktop footer into a clear brand/navigation row, utility row, and credit row with larger typography.
- Added Pictogrammers comment icons and real Blogger response counts to home cards and article actions.
- Restored Blogger native threaded comment rendering and reply editor placement; retained browser-local Like controls.
- Removed visible RSS links from the left rail, sidebar, article, and site footer.
- Verified a reply editor opens under an existing live comment and accepts text without publishing a test reply.
- Kept all eight sections, nine widgets, and stored gadget settings.

## 1.3.0 — 2026-11-14

- Audited Medium's mobile article and article footer, then adapted the hierarchy with Saeium identity and real Blogger content.
- Added publication and author context, topic chips, reading time, browser Listen, native Share, image cover, writer and publication cards, and larger related story cards.
- Restored Blogger's embedded, typeable comment form and added a styled response list with browser-local Like controls.
- Added Profile to the left rail, replaced the open hamburger with an X, removed its active background, and removed arrow labels.
- Increased home card typography on desktop and mobile.
- Verified live home, article, footer, profile, menu, and comment typing; preserved eight sections and nine widgets.

## 1.2.0 — 2026-11-14

- Matched the supplied mobile reference states for home feed, navigation drawer, and search.
- Added a truthful Saeium discovery ribbon to mobile pages.
- Added mobile For you and Featured tabs using actual posts.
- Added browser-local recent searches and a full mobile search view.
- Added Pictogrammers SVG icons to navigation and story/article actions.
- Kept all eight Blogger sections, nine widgets, and saved Link List settings.
- Checked live mobile home, menu, search, article, footer, and save action.

## 1.1.0 — 2026-11-14

- Added a persistent desktop navigation rail and a mobile drawer.
- Shortened the home introduction so stories appear earlier.
- Expanded the right rail with recent stories, local saved stories, and quick links.
- Filled story excerpts from the public Blogger feed when Blogger's snippet output is empty.
- Added article save/share actions, author panel, related stories, and a fuller footer.
- Preserved existing Blogger section and widget IDs and existing Link List settings.

## 1.0.0 — 2026-11-14

- Initial Saeium Blogger theme
- Editorial homepage, responsive story lists, article and static page styling
- Native Header, Link List, Labels, HTML, and Blog Posts gadgets
- Search panel and mobile navigation
- Built-in filtered archive with native Blogger fallback
- English installation and customization documentation
