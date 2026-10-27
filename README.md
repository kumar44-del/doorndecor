# Door N Decor — complete working website

This folder contains the actual Claude single-page website, the supplied company logo, a text-free homepage banner, and **26 product gallery photographs**.

## Run in VS Code / Chrome

1. Extract the whole ZIP. The `assets` directory must sit beside `index.html`.
2. Open the extracted **Door_N_Decor_Complete_Website** folder in VS Code.
3. Right-click `index.html` and choose **Open with Live Server**, or open `index.html` directly in a browser.
4. The home banner, header/footer logo, product cards, and category-filtered project gallery should now be visible. You do NOT need to rename any images.

Expected structure:

```
Door_N_Decor_Complete_Website/
├── index.html
├── README.md
├── IMAGE_MANIFEST.csv
└── assets/
    ├── logo.png
    ├── logo-original.jpeg
    ├── homepage-banner.jpg
    ├── homepage-banner-with-text.jpg (provided, not used)
    ├── wooden-door-01.jpg ... wooden-door-15.jpg
    ├── modular-kitchen-01.jpg ... modular-kitchen-04.jpg
    ├── wardrobe-01.jpg ... wardrobe-04.jpg
    └── window-01.jpg ... window-03.jpg
```

## Notes

- `homepage-banner.jpg` is your provided **text-free** split door-and-kitchen image. The different image called `homepage-banner-with-text.jpg` is included as an unused reference only.
- `logo.png` is created from your supplied `logo.jpeg`: only its surrounding solid black background was made transparent so the white lettering is visible over the dark header/footer. The untouched source is saved as `logo-original.jpeg`.
- The gallery includes **15 doors, 4 kitchens, 4 wardrobes, and 3 window photographs**. The two blue wardrobe photos are slightly different supplied versions and are both included as requested.
- All project photos are converted to web-friendly JPEG files, preserving the image content and original aspect ratios with no AI generation, retouching, or crop.
- Some product groups such as wallpaper and aluminium doors have no matching photo in the files provided. These show clearly labeled, non-deceptive placeholders. They are not missing assets.
- All CSS and JavaScript remains inline inside `index.html`; the photos remain external assets for normal website performance.
- All project photo names, paths, and data are stored in `const PROJECTS` near the bottom of `index.html`. They correspond exactly to the `assets` files.

## Add more project photos

Add a JPEG into `assets`, then create a uniquely numbered object in the `PROJECTS` array in `index.html`. Use `category` equal to `wooden-doors`, `kitchens`, `wardrobes`, `windows`, or `other`. Update the relevant product card image ID if appropriate.

## Publish

Upload `index.html` AND the whole `assets` directory to your hosting root, keeping the folder structure. Do not upload the ZIP itself unless your host extracts it for you.
