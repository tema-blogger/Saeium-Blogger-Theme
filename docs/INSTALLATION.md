# Installation

## Requirements

- A Blogger blog with access to **Theme** and **Layout**
- Public Blogger post feeds enabled if you want the enhanced archive filters
- At least one published post to populate story lists

## Back up your current theme

Open **Blogger → Theme → More → Backup** and download your current XML. Keep that backup until you have finished checking Saeium on your blog.

## Upload Saeium

1. Open **Theme → More → Restore**.
2. Upload `Saeium-v1.1.0.xml`.
3. Visit your public blog and refresh the page.
4. Check the homepage, one article, a label page, a keyword search, a static page, and an invalid URL.

## Configure Layout

Open **Layout**. The sections are numbered from top to bottom:

1. **Header & Logo** — use the native Header gadget to set a title or upload a logo.
2. **Main Navigation** — edit the native Link List in the left rail; the initial links are Home and Archive. Stories, Topics, and RSS shortcuts follow below.
3. **Home Introduction** — edit the HTML/JavaScript gadget. If empty, Saeium shows its sample heading and button.
4. **Topic Navigation** — choose which Blogger labels to display.
5. **Main Content** — configure the Blog Posts gadget and the number of posts per page.
6. **Sidebar** — change the short introduction and displayed labels. Fresh Reads comes from the public post feed. Saved stories are local to each visitor's browser.
7. **Footer Links** — edit the native Link List.
8. **Footer Credit** — change the copyright line if needed.

The theme does not create posts or labels for you. The live demo includes four original sample posts; mock screenshots show fictional preview content.

## Check the archive

Open `https://YOUR-BLOG/search?view=index`. It should show an archive with date and topic filters. If the enhanced archive cannot load the public post feed, it offers the native Blogger archive fallback. Keep feeds enabled in **Settings → Site feed** for the enhanced view.

## Updating

Back up the installed theme before replacing it. Use a release with a higher version number for future updates. Version 1.1.0 preserves the v1.0.0 widget and section IDs; Blogger should retain saved gadget settings, but review Layout after restoring a theme. Recent stories, article recommendations, and empty excerpts use the public Blogger post feed, so leave **Settings → Site feed** enabled.
