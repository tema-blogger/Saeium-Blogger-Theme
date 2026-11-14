# SEO for Saeium and Blogger posts

Saeium provides article markup, descriptive links and image alt text, and keeps Blogger's built-in canonical URLs and Open Graph tags. Version 1.6.1 adds a document language from the Blogger blog locale, article-first page titles, `og:type`, a Twitter card hint, and richer visible Article microdata for author, publisher, dates, URL, and cover image. The theme cannot guarantee search rankings or indexing.

## Blogger settings

1. In **Settings → Basic**, select the language used by most posts. The Saeium demo's articles are in English, so its blog language should be English.
2. In **Settings → Privacy**, keep **Visible to search engines** enabled for a public blog.
3. In **Settings → Meta tags**, enable **Search description** and write a short description of the entire blog. This supplies the homepage summary.
4. In every post's editor, open **Search description** and write a unique sentence about that article. Avoid repeating the blog-wide description or image credits.
5. Add relevant labels, descriptive H2/H3 headings, and alt text to meaningful images. Use a clear title that describes the article.
6. Connect the blog to **Google Search Console** and submit Blogger's sitemap from the blog's own domain. Do not add duplicate canonical or description tags in HTML gadgets.

Google may choose its own search snippet even when a description is supplied. Blogger already creates canonical and Open Graph URL/title/image tags; Saeium does not duplicate them.

## Article description examples for the live demo

These are editorial suggestions; each can be changed in the post editor:

| Article | Search description |
| --- | --- |
| A Conversation Is Not an Interruption | A thoughtful conversation can change the direction of an ordinary day. Learn why making time to listen can be more useful than staying on schedule. |
| An Ordinary Morning Is Enough | A good morning does not need a perfect routine. Find small ways to make an ordinary start feel calmer and more like your own. |
| A Walk Without a Destination | Walking without an errand gives your mind space to catch up. Explore how an unplanned walk can restore attention and spark ideas. |
| Making Technology Feel Human Again | Better technology helps us complete tasks while protecting our attention. Explore how to design and use tools that feel more human. |
| Reading Without a Finish Line | Reading is more than a count of finished books. Rediscover the value of slowing down, following curiosity, and remembering what matters. |
| The Case for an Unfinished Notebook | An unfinished notebook can hold quiet ideas before they disappear. Learn how simple notes become a practice of attention and creativity. |

## Check a published page

View the rendered page source and check that a post has one canonical URL, a useful description, a descriptive title, and the intended cover image. Confirm that the visible article supplies an H1, author, publication date, and meaningful subheadings. Use Google's Rich Results Test and Search Console URL Inspection to check the final published URL, then allow time for recrawling.

## Official references

- [Blogger: help people find your blog](https://support.google.com/blogger/answer/41373)
- [Blogger: manage blog settings](https://support.google.com/blogger/answer/9691230)
- [Google Search Central: Article structured data](https://developers.google.com/search/docs/appearance/structured-data/article)
- [Google Search Central: good meta descriptions](https://developers.google.com/search/docs/appearance/snippet)
- [Google Search Central: image SEO](https://developers.google.com/search/docs/appearance/google-images)
