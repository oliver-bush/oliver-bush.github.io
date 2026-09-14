# Putting this site on GitHub Pages

## What's in this folder

```
index.html          Home
research.html       Research (working papers, publications, policy research)
cv.html             CV page (embeds the PDF)
404.html            Not-found page
assets/css/style.css
assets/img/oliver-bush.jpg
files/cv-oliver-bush.pdf
```

## Step 1 — the CV is already in place

`files/cv-oliver-bush.pdf` is your 14 September 2026 CV. To swap in a newer
version later, replace that file keeping the exact same filename.

## Step 2 — create the repository

1. Sign in at github.com, click **+** (top right) -> **New repository**
2. **Repository name:** `oliver-bush.github.io`
3. **Public**
4. Do **not** tick "Add a README file"
5. **Create repository**

## Step 3 — upload the files

On the empty repository page, click **uploading an existing file**
(the link in "...or upload an existing file").

Then drag in, from inside this folder:

- `index.html`, `research.html`, `cv.html`, `404.html`
- the `assets` folder
- the `files` folder (with your CV PDF inside)

Do **not** upload this DEPLOY.md file — or do, it doesn't matter, it just
won't be part of the site.

Important: drag the **contents** of this folder, not the folder itself.
`index.html` must end up at the top level of the repository, not inside a
subfolder — otherwise the site won't load.

Scroll down, click **Commit changes**.

## Step 4 — turn on Pages

1. In the repository, go to **Settings** -> **Pages** (left sidebar)
2. Under "Build and deployment", **Source** should be **Deploy from a branch**
3. **Branch:** `main`, folder `/ (root)` -> **Save**

Wait 1–2 minutes. Your site is then live at:

    https://oliver-bush.github.io

For a repo named `oliver-bush.github.io`, Pages usually enables itself
automatically and Step 4 is just a check.

## Step 5 — updating it later

Two ways:

- **In the browser:** open the file in GitHub, click the pencil icon, edit,
  commit. Good for fixing a paper status or adding a link.
- **Replacing a file:** go to the folder, **Add file** -> **Upload files**,
  drag the new version in with the same filename, commit. This is how you
  swap in a new CV PDF.

Changes go live in about a minute.

## Optional — a custom domain

If you buy something like `oliverbush.com`:

1. At your registrar, add these DNS records:
   - Four **A** records for `@` pointing to `185.199.108.153`,
     `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One **CNAME** record for `www` pointing to `oliver-bush.github.io`
2. In GitHub: **Settings** -> **Pages** -> **Custom domain**, enter the
   domain, **Save**, then tick **Enforce HTTPS** once it becomes available
   (can take up to 24 hours).

A name-based domain looks better on applications than a github.io URL, but
github.io is perfectly respectable and costs nothing.

## Already done

The canonical and social-preview tags are set to `https://oliver-bush.github.io`.
If you later move to a custom domain, find-and-replace that string in the
HTML files.
