# Static Link Landing Page

A simple LinkTree-style static page built with HTML and CSS. Customize [index.html](index.html) with your own avatar, social profiles, and featured links, then open it directly in a browser or host it on any static site service.

## Features
- Compact, centered layout with a vertical link stack.
- Gradient background and rounded link cards with drop shadows.
- FontAwesome brand icons for social links.
- Google Fonts (Sixtyfour, Roboto Slab, Roboto, Raleway, Silkscreen) for typography.
- Thumbnail support for each link item.

## Project Structure
- [index.html](index.html) — Main page markup and embedded styles.
- `/thumbnails/` — Image assets used for the avatar and link thumbnails (e.g., `bbdevelops-imgt.svg`, `mooc-fi.png`, `rive_logo.svg`).

## Setup
1. Open [index.html](index.html) in your browser to view the page.
2. If hosting, place `index.html` and the `/thumbnails/` folder on your static host (GitHub Pages, Netlify, Vercel, etc.).

## Customization
- **Avatar**: Replace `/thumbnails/bbdevelops-imgt.svg` in the `<img class="avatar">` tag with your own image.
- **Name & Title**: Edit the `<h1>` in the `.name-row` and the subtitle in `.link-text-2`.
- **Social Icons**: Update the links and FontAwesome brand icons inside `.social-icons-row`. You can find icons at [FontAwesome](https://fontawesome.com/search).
- **Links List**: Each `.link` block contains a thumbnail and anchor. Swap the image source and `href` with your destinations. Example structure:
  ```html
  <div class="link">
    <img src="/thumbnails/example.png" class="thumbnail" alt="">
    <a class="link-text" target="_blank" href="https://example.com">
      Link label text
    </a>
  </div>
  ```
- **Colors & Typography**: Adjust gradients, card colors, and font stacks in the `<style>` block within [index.html](index.html).

## Running Locally
- Double-click [index.html](index.html) to open it in your default browser.
- For live reload or CORS-safe file loading, run a lightweight server (e.g., `npx serve .`).

## Assets
Place your replacement images in `/thumbnails/` and ensure the `src` attributes in [index.html](index.html) point to the correct filenames.

## License
Some rights reserved — see [LICENSE.txt](LICENSE.txt).
