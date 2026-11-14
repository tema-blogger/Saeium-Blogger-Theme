# Customization

Saeium v1.6.0 uses Blogger's native **Layout** gadgets. Gadget changes are saved in Blogger and appear on the live blog without editing the XML.

## Appearance and behavior

Open **Layout → 00 · Pengaturan Saeium → Theme settings**. Enter `key=value` pairs separated by semicolons:

```text
accent=#1f7a4d;ink=#242424;paper=#ffffff;readingWidth=720;articleSize=20;articleSizeMobile=19;uiFont=inter;articleFont=source-serif;relatedCount=4;readingProgress=on;showRelated=on
```

| Setting | Allowed values | Default |
| --- | --- | --- |
| `accent`, `ink`, `paper` | Three- or six-digit hex color | `#1f7a4d`, `#242424`, `#ffffff` |
| `readingWidth` | 600–850, in pixels | `720` |
| `articleSize` | 18–24, in pixels | `20` |
| `articleSizeMobile` | 17–23, in pixels | `19` |
| `uiFont` | `inter`, `arial`, `system` | `inter` |
| `articleFont` | `source-serif`, `georgia` | `source-serif` |
| `relatedCount` | 1–6 | `3` |
| `readingProgress`, `showRelated` | `on` or `off` | `on` |

The live demo sets `relatedCount=4`. Optional text settings are `featuredTitle`, `latestTitle`, `relatedTitle`, `recentTitle`, `savedTitle`, and `followLabel`. For example, append `;relatedTitle=More to read;followLabel=Follow Saeium`. Section heading values accept up to 70 characters; the follow label accepts up to 40. Gadget titles are changed in their own Layout forms. Inter and Source Serif Pro load from Google Fonts with fallback fonts; Medium's proprietary font is not bundled.

## Layout map

| Section | Gadget and purpose |
| --- | --- |
| 01 · Header & Logo | Header: blog title or uploaded logo |
| 02 · Menu Utama | Link List: primary left-rail links |
| 03 · Tautan Jelajah | Link List: additional left-rail links |
| 04 · Pembuka Beranda | HTML/JavaScript: homepage heading, description, button |
| 05 · Navigasi Topik | Labels: topic navigation |
| 06 · Postingan Blog | Blog Posts: post count and Blogger post options |
| 07 · Sidebar & Ikuti Blog | HTML/JavaScript and Labels: introduction, topics, follow copy |
| 08 · Deskripsi Footer | HTML/JavaScript: footer tagline |
| 09 · Tautan Footer | Link List: footer navigation |
| 10 · Tautan Footer Tambahan | Link List: footer shortcuts |
| 11 · Kredit Footer | HTML/JavaScript: credit text |

Link List forms let you edit each label, destination, and order. Relative paths such as `/`, `/search`, and `/search?view=index` work on Blogspot and custom domains. Automatic Profile and Follow blog links use the current Blogger blog. No RSS link appears in the theme.

## Home introduction

Open **04 · Pembuka Beranda → Home introduction**. Leave it empty for the built-in copy, or add HTML:

```html
<h2>Your stories begin here.</h2>
<p>A short description of what readers can expect.</p>
<a class="pill" href="#stories">Start reading</a>
```

The introduction appears on desktop home pages. On mobile, the post feed starts below the For you and Featured tabs.

## Posts, photos, and related stories

Set each article's first image in the Blogger post editor. Cards and article covers use Blogger's image output. Related stories read the full public post feed; if no feed thumbnail exists, Saeium uses the first image from the post body. A genuinely imageless post keeps the neutral placeholder. Related images load lazily, and covers link to their articles. Blogger labels help rank stories with shared topics first.

The six demo posts have hidden first source images used for cover metadata. Those source images use `loading="lazy" decoding="async"` to avoid an unnecessary full-size download. A normal visible first image in your own post needs no special markup.

The article header includes a title, topics, date, subtitle derived from the opening paragraph, read time, author, and cover. Listen uses browser speech synthesis. Share uses the native share sheet where available or copies the URL. Saved stories and comment Likes are stored in each visitor's browser, not a shared account.

## Follow and comments

Follow blog controls open Blogger's official confirmation and add posts to the follower's Blogger Reading List; this is not an email subscription. Set **Settings → Comments → Comment location** to **Embedded** and leave per-post comment feeds enabled. Blogger provides the editor and threaded replies. Some browsers require third-party cookies for Google sign-in. The Like button is a browser-local toggle, not a public vote total.

## Search, archive, and footer

Search opens Blogger's `/search?q=...`. Mobile recent searches are stored locally. The archive at `/search?view=index` offers date and topic filters when the public feed is enabled, otherwise it falls back to Blogger's native archive. Its default timezone is `Asia/Jakarta`; changing that adapter requires editing and rebuilding the XML.

Edit sections **08–11** for the footer tagline, two link groups, and credit. On desktop, the brand and primary links occupy the top row, utility links the next row, and credit sits below a divider. On mobile, the hamburger becomes an X while the drawer is open. Home cards and article actions show Blogger's comment count.
