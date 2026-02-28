# Live Class YouTube Embed Page

A simple static web page that presents a live class-style layout and embeds a YouTube video.

## Files
- `index.html` – page structure and embedded YouTube iframe
- `styles.css` – responsive styling

## Host locally

From this folder:

```bash
python -m http.server 4173
```

Then open:

- `http://localhost:4173`

## Host publicly (GitHub Pages)

1. Push this repository to GitHub.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` (or your default branch), folder `/ (root)`
4. Save and wait for deployment.
5. Your page will be available at:
   - `https://<your-username>.github.io/<repo-name>/`

## Host with Nginx using Docker

```bash
docker build -t live-class-page .
docker run --rm -p 8080:80 live-class-page
```

Open:

- `http://localhost:8080`
