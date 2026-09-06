# Todo List

A simple to-do list website built with plain HTML, CSS, and JavaScript. No frameworks, no build step — just three files.

## Features

- Add tasks
- Mark tasks complete / incomplete
- Delete tasks
- Filter by All / Active / Done
- Clear all completed tasks
- Tasks are saved in the browser (`localStorage`), so they persist after you close the tab

## Files

```
index.html   - page structure
style.css    - styling
script.js    - task logic (add, complete, delete, filter, save)
README.md    - this file
```

## Running it locally

You don't need any server or install step. Just open `index.html` in a browser:

- Double-click `index.html`, or
- Right-click it and choose "Open with" your browser

That's it — the app works fully offline since everything runs in the browser.

## Deployment

Since this is a static site (just HTML/CSS/JS, no backend), you can host it for free on any of the following. Pick whichever is easiest for you.

### Option 1: GitHub Pages (free, no account needed beyond GitHub)

1. Create a free account at [github.com](https://github.com) if you don't have one.
2. Create a new repository (e.g. `todo-list`).
3. Upload `index.html`, `style.css`, and `script.js` to the repository (use "Add file" → "Upload files" on the repo page, or `git push` if you're comfortable with Git).
4. Go to the repository's **Settings** tab → **Pages** (in the left sidebar).
5. Under "Build and deployment", set **Source** to "Deploy from a branch", choose the `main` branch and `/ (root)` folder, then click **Save**.
6. Wait a minute or two, then GitHub will show you a live URL like:
   `https://your-username.github.io/todo-list/`

### Option 2: Netlify (free, drag-and-drop, no Git required)

1. Go to [netlify.com](https://www.netlify.com) and sign up (free).
2. After logging in, go to your dashboard and look for a "drag and drop" upload area (usually on the Sites page).
3. Drag your project folder (containing `index.html`, `style.css`, `script.js`) directly onto that area.
4. Netlify uploads the files and gives you a live URL immediately, like:
   `https://random-name-123.netlify.app`
5. Optional: rename the site or connect a custom domain from the site settings.

### Option 3: Vercel (free, similar to Netlify)

1. Go to [vercel.com](https://vercel.com) and sign up (free).
2. Click "Add New" → "Project".
3. You can either connect a GitHub repo (see Option 1 to create one first) or use the Vercel CLI to deploy a local folder.
4. Vercel builds and gives you a live URL like:
   `https://your-project.vercel.app`

### Option 4: Any basic web host

Since this is just static files, you can also upload `index.html`, `style.css`, and `script.js` via FTP/File Manager to any traditional web hosting provider (e.g. cPanel-based hosting) — just place them in the public folder (often called `public_html` or `www`).

## Notes

- No build tools, npm, or dependencies are required — the three files are the entire app.
- Because tasks are stored in `localStorage`, they are saved per-browser/per-device. Opening the site on a different device or browser will start with an empty list.
- Everything runs client-side, so any of the free static hosts above work with zero configuration.
