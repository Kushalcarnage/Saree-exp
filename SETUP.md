# Vijayalakshmi Silk Palace — website package

## What's inside
| File / folder | What it is |
|---|---|
| `index.html` | The website. |
| `media/` | Product photos, store photos and the two videos. |
| `vendor/` | The AI try-on models (body detection and person outline). Don't rename or delete. |
| `fabric-marker.html` | Helper page for adding new sarees (see below). Not linked from the site. |

## Putting the website online
Upload **everything** (index.html, media/, vendor/) to the website hosting, replacing the old site files.
The site must open with **https://** — phones only allow the camera on secure sites. Most hosting gives this free.

The AI try-on needs **no account, no server and no fees**. It runs on each customer's own phone or computer,
and the camera picture never leaves their device.

## Adding a new saree (no coding)
1. Open `fabric-marker.html` in Chrome on a computer.
2. Choose the saree photo (laid flat or folded, straight from above, in daylight).
3. Drag a box over the plain body fabric, then a box over the border. Check the previews look even.
4. Fill in the code (e.g. p17 — must be unique), name, collection, colours and price (empty = "Price on request").
5. Click **Download website photo** → put the file in the `media/` folder.
6. Click **Copy saree entry** → open `index.html` in a text editor (Notepad is fine), find `window.SAREES = [`
   and paste on the next line. Save.
7. Upload the photo and index.html to the hosting.

To change a price or name later, edit that saree's line in `index.html` the same way.
To remove a saree, delete its lines (from `{ id:` to the closing `},`).

## Contact details
Phone numbers, WhatsApp number, address and social links are in `window.STORE` near the top of the site data in index.html.
