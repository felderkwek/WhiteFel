# WhiteFel Apps

A static app hub for **Mac Sweeper** and **Little Reel**, built for the existing GitHub Pages repository. Plain HTML and CSS; no build tooling, external fonts, analytics scripts, or runtime dependencies.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | WhiteFel app hub |
| `little-reel/index.html` | Little Reel product page |
| `little-reel/support.html` | Little Reel support and contact information |
| `little-reel/privacy.html` | Little Reel privacy policy draft |
| `mac-sweeper/index.html` | Original Mac Sweeper product page |
| `support.html` | Existing Mac Sweeper support URL |
| `privacy.html` | Existing Mac Sweeper privacy URL |

The root homepage becomes the app hub. Existing Mac Sweeper support and privacy addresses remain valid. The original product content is retained under `mac-sweeper/`. The placeholder privacy contact was replaced with the existing public support address, `felderkwek@gmail.com`.

Little Reel is shown as **coming to the App Store**, with a **one-time purchase**, **no ads**, and no announced price. No inactive App Store download buttons are included.

## Publish

Publish the repository’s root through its existing GitHub Pages configuration. Merge the `feat/whitefel-app-hub` branch into `main`, then wait for the Pages deployment to finish. This change does not add a new hosting service or change the repository name.

Before release, read `APP-STORE-HANDOFF.md`, check the privacy policy against the actual submission build, and add the real App Store product URL when available.

If you are using the downloadable website package, copy its contents into your existing repository checkout, commit the changes with GitHub Desktop or Git, and publish through the repository’s current Pages configuration. Put `index.html` at the repository root, rather than inside an extra enclosing directory. Keep the `assets`, `little-reel`, and `mac-sweeper` directories together with it.

## Adding another app

1. Add a directory for the app, with product, support, and privacy pages.
2. Add its icon or screenshots under `assets/`.
3. Add a new app entry to the collection in `index.html` and its support link below.
4. Add its public page URLs to `sitemap.xml`.

Use relative asset and navigation paths so pages work under the repository’s `/macsweeper-site/` base path. The custom `404.html` uses that base path explicitly.

## Verification

Checked the eight HTML pages for local links, images, fragment anchors, one main heading, duplicate IDs, contact placeholders, and inactive download links. Parsed the sitemap. Browser checks covered desktop pages, mobile widths of 390px and 320px, and the expandable support FAQs. No JavaScript is required for the site.

Original Mac Sweeper content is retained from repository commit `c0114d0e6f551f68fe0bf383f24340b8423ef789`. Little Reel artwork and screenshots are existing project assets supplied in the conversation.
