# Little Dreams TV

A free, child-friendly learning site made installable as a web app. It keeps the existing Little Dreams TV look, the ABC & First Words, Music & Rhymes, Story Garden, and Play & Discover sections, and the featured YouTube lesson.

## What changed

- Added an app manifest and Little Dreams TV icons so supported browsers can add the app to a phone's home screen.
- Added a small offline page cache. After the first online visit, the page and its built-in learning activities can open without a connection. YouTube videos, web-hosted photos, and web fonts still need internet.
- Added an in-page Install app button on browsers that offer an install prompt, plus a notice when the device is offline.
- No paid service, app-store account, or build tools are needed.

## Put it on a phone

The app needs a secure website address (HTTPS) to install. This public repository already has a GitHub Pages workflow at `.github/workflows/static.yml`.

1. Merge the app changes into the `main` branch.
2. In GitHub, open **Settings → Pages** and select **GitHub Actions** as the publishing source if it is not already selected.
3. Wait for the **Deploy static content to Pages** workflow to finish. Its successful run shows the website address.
4. On Android, open that address in Chrome and choose **Install app** (or the browser menu's install option).
5. On iPhone, open the address in Safari, tap **Share → Add to Home Screen**, then turn on **Open as Web App** if that option appears.

GitHub Pages is available at no charge for public repositories on GitHub Free. See [GitHub Pages setup](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) and [GitHub Pages availability](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits).

## Preview on a computer

You can open `index.html` to look around, but browser installation and offline caching need HTTPS or a local web server. If Python is installed, open a terminal in this folder and run:

```text
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Add more original videos later

The featured alphabet video is already embedded. To add another original video, add its YouTube embed to the **Welcome to our video corner** section in `index.html`, or add a link to the topic cards. Keep the videos on YouTube; the app streams them and does not copy video files into the repository.
