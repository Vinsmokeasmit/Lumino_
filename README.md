# Lumen – Photographer Portfolio (frontend)

Each page is its own HTML file with its CSS and JS inside it.

| File | Use |
|---|---|
| index.html | Home: hero, photographers, latest work |
| explore.html | Search and filter all photos |
| login.html | Log in |
| signup.html | Create account (photographer or viewer) |
| upload.html | Photographers upload to Cloudinary |
| portfolio.html?u=username | A photographer's public portfolio |

Run: open index.html, or serve the folder (npx serve .).

## Cloudinary
In each page's script, the CLOUDINARY block (only upload.html uses it) takes:
- cloudName
- uploadPreset (UNSIGNED preset)
Never put your API secret in frontend code.

Demo account: miraj@demo.com / demo1234

Shared code (styles, DB store, nav, lightbox) is repeated in each file by design. Users, photos and session live in localStorage via the DB object until the backend exists.
