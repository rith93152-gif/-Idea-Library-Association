# ILA Reader Club Website

Static website for **ILA Reader Club / Idea Library Association**.

## Technology

- HTML pages at the repository root
- CSS in `assets/css/`
- JavaScript in `assets/js/app.js`
- Mock content in `assets/data/site-data.json`
- Browser-only join applications stored in `localStorage`

There is no PHP, MySQL database, server-side backend, login system, or admin dashboard. This makes the site compatible with GitHub Pages.

## GitHub Pages

1. Push this repository to GitHub.
2. Open **Settings → Pages**.
3. Select **Deploy from a branch**.
4. Choose the default branch and the repository root (`/`).
5. Save and open the generated Pages URL.

The home page is [index.html](index.html).

## Local preview

Because the site loads JSON with the Fetch API, serve the folder through a local web server instead of opening the HTML file directly.

For example, with Python installed:

```powershell
py -m http.server 8000
```

Then open `http://localhost:8000/`.

## Content updates

Edit [assets/data/site-data.json](assets/data/site-data.json) to update members, events, news, gallery items, or organization information. Reload the page after saving the JSON file.

The join form does not send data to a server. It saves submissions in the visitor's browser under the `ilaJoinApplications` localStorage key. LocalStorage data is private to that browser and is not a replacement for a shared production database.

## Pages

- [Home](index.html)
- [About](about.html)
- [Events](events.html)
- [News](news.html)
- [Gallery](gallery.html)
- [Members](members.html)
- [Member profile](member.html?id=1)
- [Join](join.html)
