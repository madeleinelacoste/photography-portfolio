MADELEINE LACOSTE PHOTO PORTFOLIO — VS CODE VERSION

Open this folder in Visual Studio Code, then open index.html in a browser.
For easier live previewing, the VS Code “Live Server” extension is convenient but not required.

FILES
- index.html ............ page content and photo order
- styles.css ............ layout, typography, spacing, hero height, gallery styling
- script.js ............. lightbox behavior and automatic copyright year
- assets/hero.jpg ....... tall Morocco background/hero image
- assets/madeleine-lacoste-title.png ... handwritten title graphic
- assets/gallery/ ....... all 67 portfolio photos (the page order is set in index.html, not by file number)
- single-file-backup.html ... backup of the self-contained version you liked

MOST COMMON EDITS

1. ABOUT ME
Search index.html for:
    EDIT ABOUT-ME TEXT BELOW
Change the <h2> and <p> text there.

2. CONTACT
Search index.html for:
    EDIT CONTACT DETAILS BELOW
Replace you@example.com, the Instagram link (#), and the location text.
Example Instagram link:
    <a href="https://www.instagram.com/yourusername/" target="_blank">Instagram</a>

3. PHOTO DESCRIPTIONS / LIGHTBOX CAPTIONS
Each gallery <img> has a data-caption attribute in index.html.
Example:
    data-caption="Marrakech, Morocco"
Whatever you type there will appear beneath the enlarged photo in the lightbox.
Also update alt="..." for accessibility/search engines.

4. HERO HEIGHT
In styles.css, search for:
    .hero
The current tall hero uses:
    min-height:max(100svh,139.42vw)
This is intentionally tall so the portrait background image can be seen almost in full before the grid begins.

5. PHOTO ORDER
The gallery order is controlled entirely by the order of the photo-card buttons in index.html.
Rows are grouped into landscape-row and portrait-row classes so each row stays visually consistent.

IMPORTANT
Keep the folder structure intact when moving/publishing the site, because index.html references the images using relative paths.
You do NOT need the original font file: the handwritten name is stored as a PNG graphic in assets/.
