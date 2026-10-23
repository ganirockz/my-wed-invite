# Ganesh & Jaya Sai Pragnya Wedding Invitation

A responsive, static wedding invitation built with HTML, CSS, and vanilla JavaScript. A muted opening video leads into the welcome slide, where guests can start or pause the wedding background music, followed by the invitation details, event schedule, and responsive Google Maps embed.

## Run locally

From this folder, run:

```sh
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000). A local server is needed so the Three.js module, map, and invitation scripts load consistently.

## Customize wedding details

Edit [`wedding-details.js`](wedding-details.js) to update the couple and parents, event schedule, ceremony time, venue address, and map search. The site currently reflects the Telugu invitation date, **15 November 2026**, and Ganesh's confirmed **9:14 PM IST** muhurtham. The PDF's English date and time differ from its Telugu date line and the later time confirmation; confirm the date before sharing the final invitation if the English month was intended.

The map and both directions buttons use the supplied Google Maps location link. Update `mapUrl` in `wedding-details.js` if the destination changes; `mapQuery` remains the fallback search location.

## Deploy with GitHub Pages

1. Commit and push the project to the repository's `main` branch.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**, then choose **main** and **/(root)**.
4. Save and open the published URL shown on the Pages settings screen.

No build step is needed. Use a custom domain through the same Pages settings if desired.

## Assets

- `assets/wedding-opening.mp4` and `assets/lord-ganesha-mobile.mp4` — desktop and mobile opening videos.
- `assets/wedding-background.mp3` — the background music track.
- `assets/wedding-welcome.jpeg` — the couple artwork on the welcome slide.
- `assets/ganesha-logo.jpeg`, `assets/lord-venkateswara-logo.jpeg`, and `assets/lord-shiva-parvathi-devi-logo.jpeg` — the family blessing logos.

The page currently has no RSVP section, as requested.
