# Personal website — Dr. Laura Bravo Merodio

A single-file personal CV / portfolio website (Assistant Professor in Health Data Science & Computational Biology, University of Birmingham).

Everything lives in `index.html` — no build step, no dependencies. Just open the file in a browser.

## Publish it free with GitHub Pages

The repo is at https://github.com/InFlamUOB/webpage. From this folder, run:

```bash
git init
git add .
git commit -m "Add personal website"
git branch -M main
git remote add origin https://github.com/InFlamUOB/webpage.git
git push -u origin main
```

If the repo already exists and is empty, skip `git init`/`git branch` and just `git remote add` + `git push`.

Then turn on Pages:

1. Go to **https://github.com/InFlamUOB/webpage** → **Settings** → **Pages**
2. Under **Build and deployment → Source**, choose **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)** → **Save**
4. Wait ~1 minute. Your site will be live at:

   **https://inflamuob.github.io/webpage/**

> Tip: for a cleaner URL (`https://inflamuob.github.io/`), name the repo `InFlamUOB.github.io` instead of `webpage`.

## Editing

All content is plain HTML inside `index.html`. Search for a section heading (e.g. `<!-- PUBLICATIONS -->`) and edit the text directly. The styling lives in the `<style>` block at the top — change `--navy` and `--coral` to recolor the whole site.

## Customising the avatar

The circular badge currently shows your initials ("LB"). To use a photo, replace:

```html
<div class="avatar">LB</div>
```

with:

```html
<img class="avatar" src="profile.jpg" alt="Laura Bravo Merodio" />
```

and drop a `profile.jpg` into this folder.
