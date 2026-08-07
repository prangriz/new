# prangriz.github.io

Minimalist personal homepage. Plain HTML + CSS, no build step, no framework — GitHub Pages serves it as-is.

## Structure

```
index.html          home / about
publications.html   publications list
teaching.html        teaching list
style.css            shared stylesheet
cv.pdf                (add your own CV here — index.html links to it)
```

## Editing

- Bio and news: edit the `<section id="about">` and `<section id="news">` blocks in `index.html`.
- Add a publication: copy one `<li>` block in `publications.html`.
- Add a course: copy one `<li>` block in `teaching.html`.
- Colors, type, spacing: all in `style.css` under the `:root` variables at the top.

## Deploying

This is meant to replace the contents of your `prangriz.github.io` repository (the one already serving
your site at https://prangriz.github.io/).

```bash
# from inside a fresh clone of prangriz.github.io
rm -rf *                     # clear out the old Jekyll/AcademicPages site
# copy these files in
git add -A
git commit -m "Switch to minimalist static site"
git push
```

GitHub Pages will pick it up automatically — no Jekyll config, no `_config.yml`, no gems needed,
since these are already plain static files.

If you'd rather keep the old site around, push this to a new repo instead and point it at a
custom domain or a `/new` path.
