# Medium mobile article audit — 14 November 2026

Reference: https://medium.com/zenite/you-need-to-get-lost-before-you-can-find-yourself-e27bddcc2ae8

Evidence: the user's supplied iPhone screenshot and a live inspection of the linked Medium article at a 390px viewport. The supplied capture is the visual reference for the mobile header state.

## Observed article order

1. Compact utility header and narrow colored promotion band.
2. Publication identity row with a follow action, separated by a rule.
3. Story status badge, then outlined topic chips.
4. Large bold title, muted subtitle, read time and date.
5. Author avatar/name with a follow action.
6. Rounded action pills for listening, sharing and more options.
7. Full-width lead image, then serif article text.

## Footer observed on the mobile article

After the text, Medium repeats the story reactions and bookmark controls. A large author card presents the writer's name, short bio and follow action. A separate publication card follows, then a recommended-story feed with large images, publication/author metadata, bold titles, short excerpts and compact actions. The general Help/Status/About/Privacy/Rules links exist in the page DOM but are not visually laid out in the inspected mobile view. The reference also inserts a membership upsell; that commercial block is specific to Medium and is not reused.

At 390px, the live title is 32px with a 38px line height and a roughly 327px text measure; the subtitle is 18px/24px. The first lead figure spans the mobile viewport. The user's capture shows a wider gap between the publication row and title, topic chips wrapping to two rows, and action pills below the byline.

## Saeium adaptation

- Keep the Saeium brand and existing discovery ribbon. Use a truthful publication row and the official Blogger Follow blog action. Do not reproduce Medium membership claims or imply a paid story. This follow action replaced the early RSS proposal in version 1.5.0.
- Use Blogger labels as clickable topic chips, Blogger author/date, and an estimated reading time computed from article text.
- Use the first paragraph as a visual deck only when it can be moved intact from the article body; avoid duplicating article copy.
- Use a lead image from Blogger when available, with an original neutral editorial fallback when absent.
- Provide working browser speech, share and more controls where supported, retaining save and responses.
- Preserve native Blogger comments and avoid copying the referenced article, author image or artwork.
- Shape Saeium's article footer around a writer card, a publication card with its own Follow blog action, related stories and a working comment section. Keep the existing editable site footer and credit. Remove decorative arrow characters from links.

## Verification on the Saeium demo

Saeium v1.3.0 is installed at https://saeium.blogspot.com/. The article header, writer and publication cards, three related stories, and embedded Blogger comment editor were inspected at a 390px viewport. The comment textarea accepted text, and the test text was cleared without posting. At 320, 375, 390, 414, 768, and 1440px, the local render had no horizontal overflow or page-script errors.

The Like button on each comment is a browser-local preference; Blogger does not provide a theme-level shared Like total. The live demo has no published comments, so this button was interaction-tested in a local representative render.
