# 九寨沟旅行 | Chongqing and Jiuzhaigou Trip Planner

An 8-day, 6-night itinerary assistant for a trip through Chongqing, Chengdu, Huanglong and Jiuzhaigou. It is a single-page static website with a day-by-day timeline, an interactive map, and photo upload with local storage.

## Features

- Day-by-day timeline of the full itinerary
- Interactive map built with Leaflet
- Photo upload, saved in the browser (optional Firebase sync if you add your own config)
- Mobile-friendly layout styled with Tailwind CSS

## Run locally

No build step is needed. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy with GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. After a minute, the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Optional: enable Firebase sync

In `index.html`, the `myFirebaseConfig` variable is `null` by default, so photos are stored only in the visitor's browser. If you add your own Firebase config, do not commit private credentials. Firebase web config values are not secret, but you should lock down your Firestore security rules.

## Tech stack

- HTML, CSS, JavaScript
- [Tailwind CSS](https://tailwindcss.com/) (CDN)
- [Leaflet](https://leafletjs.com/) (CDN)
- [Font Awesome](https://fontawesome.com/) (CDN)
- [Firebase](https://firebase.google.com/) (optional)

## License

MIT, see [LICENSE](LICENSE).
