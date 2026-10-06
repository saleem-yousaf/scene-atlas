# DEPLOY: Scene Atlas

Same setup as your other projects. New repo, repo NAME becomes the URL path, plain GitHub
Pages serving from the branch root. No Actions workflow, no dist folder, files at the root.
Live URL after deploy: https://saleemyousaf.co.uk/scene-atlas/

## What changed from the original zip
- Removed the generator metadata folder that shipped with the build (it held a tool project id). No AI or vendor markings remain
  anywhere in the project. Verified across every file.
- Removed the bundled GitHub Actions workflow and the dist folder. The site now sits at the
  repo root and serves the same way as millers-planet and westeros-underground-map.
- Kept .nojekyll at the root. This is required so Pages serves the assets folder correctly.
- Added SEO to match the other pages: canonical, Open Graph, Twitter card, and the Person
  entity with worksFor Cyber Spartans and the full sameAs network. Added a footer links block
  to your sites, profiles and the two other fun pages.
- Replaced stray em dashes with commas per house style (title, app.js, data.js).

## Files
All files sit at the repo ROOT. index.html, style.css, app.js, data.js, photos.js,
.nojekyll, README.md, and the assets folder.

## Steps

### 1. Create the repo
1. GitHub, + then New repository. Owner: saleem-yousaf.
2. Name: scene-atlas  (lowercase, this becomes the URL path).
3. Public. Do not add a README on the create screen.
4. Create repository.

### 2. Upload everything to the root
1. "uploading an existing file".
2. Select ALL items from this pack: index.html, style.css, app.js, data.js, photos.js,
   README.md, .nojekyll, and the assets folder. Drag them in so they land at the root.
   Note: .nojekyll starts with a dot. If your file picker hides dotfiles, enable "show hidden"
   so it uploads. Without it, Pages may drop the assets folder.
3. Commit changes.

### 3. Turn on Pages (branch method, same as your others)
1. Settings, Pages.
2. Source: Deploy from a branch.
3. Branch: main, folder: / (root). Save.
4. Tick Enforce HTTPS once available. Leave custom domain blank, it inherits saleemyousaf.co.uk.

### 4. Confirm
Wait one to two minutes, open https://saleemyousaf.co.uk/scene-atlas/ and check the globe
loads and photos appear. Open "Sources and photo credits" to confirm attribution shows.

### 5. Apex repo follow-ups (in saleem-yousaf.github.io, not here)
- Add to sitemap.xml:
    <url>
      <loc>https://saleemyousaf.co.uk/scene-atlas/</loc>
      <lastmod>2026-10-06</lastmod>
      <changefreq>monthly</changefreq>
      <priority>0.8</priority>
    </url>
- Add a homepage link next to the others:
    <a href="/scene-atlas/">Scene Atlas, real movie filming locations</a>

### 6. Search Console
Domain property, URL inspect the scene-atlas URL, Request Indexing. Use Test Live URL then
View Tested Page to confirm the globe renders, since it builds in JavaScript.

## Open item (optional)
og:image points at og-image.png, which is not in the pack yet. Link previews will fall back
to no image until you add one. Say the word and I will make a Scene Atlas card in the same
poster style as the others.

## Not checked
The factual film-to-location data was not verified entry by entry. Photos are correctly
licensed and credited. A spot check of a few location claims is worth doing since it is your name on it.
