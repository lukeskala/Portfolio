# Luke Skala — Portfolio Website

A static, GitHub Pages-ready portfolio. The homepage combines a cinematic sports-broadcast introduction with an interactive project selector. No server, build tool, npm installation, or API key is required.

## Start here

1. Unzip the archive. **Keep `index.html` at the top level** alongside `replay.html`, `girlies.html`, `README.md`, and the `assets/` folder.
2. Double-click `index.html` to preview it locally. Some external content, such as the YouTube player and Google Fonts, requires an internet connection.
3. Test the buttons, project selector, and links. On mobile, use the **Menu** button.

## Publish on GitHub Pages

1. Sign in at [github.com](https://github.com) and create a new **public** repository, such as `luke-skala-portfolio`.
2. Select **Add file → Upload files** in the new repository.
3. Upload **the contents of the unzipped folder**, not the folder itself. Confirm that `index.html` appears at the repository root and `assets/` is beside it. Commit the upload.
4. Open **Settings → Pages** in your repository.
5. Under **Build and deployment**, select **Deploy from a branch**. Choose `main` and `/ (root)`, then **Save**.
6. Wait for GitHub to finish deployment. The Pages settings screen will show the published address. A typical project address is `https://YOUR-USERNAME.github.io/luke-skala-portfolio/` (replace the username and repository name with your own).
7. Open the address and test every page and media link. If the site shows a 404 initially, give deployment a few minutes and check **Actions** or **Settings → Pages** for errors.

**Important:** Uploading this ZIP does not publish anything automatically. You must complete the GitHub steps yourself.

## Files

- `index.html` — homepage, interactive selector, About, experience, audio, and contact
- `replay.html` — G-MAC championship replay case study
- `girlies.html` — *The Girlies* film case study
- `assets/style.css` — colors, typography, layout, mobile breakpoints, reduced-motion behavior
- `assets/main.js` — menu and keyboard-accessible project selector
- `assets/images/portrait.webp` — professional headshot
- `assets/images/switcher.webp` — production switcher and monitor wall
- `assets/images/viz-3play.webp` — Viz 3Play replay controller
- `assets/audio/resound-pineapple-pizza.mp3` — radio sample
- `assets/docs/Luke-Skala-Resume.pdf` — website-safe résumé without hometown/address or phone number

## Editing your content

You can edit `.html` files in GitHub's built-in editor (click a file, then the pencil icon), or in a text editor such as VS Code.

- **Change your introduction:** In `index.html`, find `Aspiring sports producer` and edit the sentence. The wording is a concise draft based on your interview; approve or revise it before using the site for applications.
- **Change the motto:** Find `pressure makes diamonds` in `index.html`.
- **Update contact links:** Search `lukeaskala@gmail.com` and `linkedin.com/in/lukeskala` across the HTML files.
- **Change the project previews:** In `assets/main.js`, edit the `projects` object. Each entry contains `title`, `role`, `desc`, `image`, `alt`, `url`, and `cta`.
- **Replace a photo:** Put a new image in `assets/images/` and update the matching `src` in HTML or `image` in `assets/main.js`. Give it meaningful `alt` text.
- **Replace the radio sample:** Replace `assets/audio/resound-pineapple-pizza.mp3` with a new MP3 using the same filename, or change the `<source src>` in `index.html`.
- **Replace the résumé:** Export your updated PDF and overwrite `assets/docs/Luke-Skala-Resume.pdf`. **Check that your phone number and address are still absent before uploading.**
- **Change colors:** Edit the CSS variables at the top of `assets/style.css` (especially `--red`, `--bg`, and `--panel`).

All internal links use **relative paths**, so they work on a GitHub Pages project URL under a repository name.

## Media notes and limitations

- **FloCollege:** The replay case study links to the full broadcast and gives the starting point **2:33:30**. It does not embed or redistribute protected footage. Viewer access may require a subscription. Add an authorized clip or verified timestamp link later if permitted.
- **The Girlies:** The page embeds the supplied YouTube link and offers a direct YouTube fallback. Availability depends on the video's privacy settings and embedding permissions. Film-specific stills have **not** been provided; the homepage uses a production equipment photo for that project card, explicitly labeled as such.
- **Résumé:** A new public PDF was typeset from the supplied résumé content with the hometown/address and phone number omitted. The original was not changed. Review all content, including dates and claims, before applying for jobs.
- **Fonts:** Google Fonts is optional. System fonts are used automatically if Google Fonts cannot load.
- **Privacy:** The website publicly displays your email and LinkedIn. Your uploaded résumé is also public to anyone with the site URL.

## Accessibility and QA

Semantic headings, a skip link, visible keyboard focus, descriptive image text, mobile navigation, project buttons with `aria-pressed`, video fallback, native audio controls, and reduced-motion styles are included. Test on your actual phone and browser after publishing.

## Adding new work

Duplicate a case study page, change its title, content, and media, then add a new link in `index.html`. If you want it as a new dashboard channel, add a fourth `projects` entry in `assets/main.js` and a matching `<button data-channel="...">` in `index.html`.
