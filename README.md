# Personal site

A bare-bones HTML/CSS site: white background, blue underlined links,
a sidebar of links on the left, no boxes or fancy styling. Built to be
easy to edit by hand, like an old Tumblr/Neocities layout.

## Files

- `style.css` — the one stylesheet all pages share. Change fonts/colors here.
- `index.html` — home page
- `cv.html` — your CV/resume
- `blog.html` — list of blog posts
- `posts/post-template.html` — copy this to make a new blog post
- `photography.html` — photo gallery
- `illustration.html` — illustration gallery
- `links.html` — links to other places you post work
- `images/photography/`, `images/illustration/` — put your images here

## Editing

Each page is a plain `.html` file — open it in any text editor.
The sidebar is the same block of code copy-pasted at the top of every page,
with the current page shown as plain text instead of a link. To add a new
page:

1. Copy an existing `.html` file and rename it.
2. Edit the `<h1>` and content in `<main>`.
3. Add a new `<li>` link to it in the sidebar of every page (including the
   new page's own sidebar, where it should be the "current" one, not a link).

To add a blog post: copy `posts/post-template.html`, rename it, fill in the
title/date/text, then add a link to it near the top of `blog.html`.

To add a photo or illustration: drop the image file into `images/photography/`
or `images/illustration/`, then add an `<img>` line to the gallery on that page.

## Putting it on GitHub Pages

1. Create a new GitHub repository (public).
2. Upload all these files and folders to it, keeping the same structure
   (so `style.css` sits next to `index.html`, `posts/` is a subfolder, etc.).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set Source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`. Save.
5. After a minute or two your site will be live at
   `https://your-username.github.io/repo-name/`.

If you want the site at the root of `your-username.github.io` (no repo name
in the URL), name the repository exactly `your-username.github.io`.
