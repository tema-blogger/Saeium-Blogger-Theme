# Customization

## Logo and title

Open **Layout → Header & Logo → Blog title and logo**. Upload a logo with little transparent padding. Saeium limits its display to 190 × 42px on desktop and 150 × 42px on small screens. Without an image, the public header shows your Blogger blog title.

## Navigation

Open **Layout → Main Navigation → Main menu**. Use the Link List form to edit the left rail's primary labels, URLs, and order. The default primary links are Home and Archive; Stories, Topics, and RSS shortcuts follow below them. Relative paths such as `/`, `/search`, and `/search?view=index` work on Blogspot and custom domains. The header hamburger collapses the desktop rail and opens a drawer on mobile.

## Home introduction

Open **Layout → Home Introduction**. If its content is empty, the theme displays a sample heading and button. To use your own text, add HTML such as:

```html
<h2>Your stories begin here.</h2>
<p>A short description of what your readers can expect.</p>
<a class="pill" href="#stories">Start reading</a>
```

The introduction appears on the homepage only. Version 1.1.0 keeps it compact so readers reach the stories sooner. Keep the heading short for mobile screens.

## Labels and story lists

Create labels on posts in Blogger. The **Topic Navigation** and **Discover topics** gadgets read those labels. The featured list on the homepage uses the first three posts in the native Blog Posts list. The main story list uses Blogger's normal post order and pagination. If Blogger provides an empty snippet, Saeium fills the card excerpt from the public post feed. Posts without a featured image use a neutral editorial placeholder.

## Right rail and article actions

The right rail starts with editable **About this blog** and **Discover topics** gadgets. **Fresh reads** and article **Keep reading** links load from the public Blogger post feed. The **Your reading list** area stores saved story links in each visitor's browser using local storage. It is not tied to a Blogger or Medium account and does not sync across devices. The article Share button uses the browser's native share sheet when available and otherwise copies the URL.

## Search and archive

The header search sends a standard Blogger keyword query to `/search?q=...`. The **Archive** link opens `/search?view=index`, which provides date and topic filters. The default archive timezone is `Asia/Jakarta` (WIB); change the index adapter configuration before rebuilding if your blog uses another publishing timezone.

## Colors and type

Edit the CSS variables at the top of the theme's `b:skin` block. The key variables are `--ink`, `--muted`, `--line`, `--paper`, `--cream`, `--accent`, and `--reading`.

Saeium uses Georgia for the large introduction and article body, and system sans-serif fonts for navigation and story cards. This keeps the theme usable without external font requests.

## Footer

Edit **Footer Links** and **Footer Credit** in Layout. The default credit is `© 2026 Tema Blogger. All rights reserved.` and links to temablogger.com. Enter your own HTML in Footer Credit to replace it.
