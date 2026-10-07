# Life Reconnect

The website for Life Reconnect (lifereconnect.ca), served by GitHub Pages.

It is plain HTML and CSS with no build step: what is in this repository is what gets published.

## Pages

| Page | File |
| --- | --- |
| Home | `index.html` |
| Contact | `contact/index.html` |
| Rates | `rates/index.html` |
| Blog | `blog/index.html` |
| Incense | `incense/index.html` |
| Post: Why the name Life Reconnect | `2020/06/23/why-the-name-life-reconnect/index.html` |
| Post: Legacy work | `2020/01/12/legacy-work/index.html` |

The folders match the addresses the pages had on the old WordPress site, so existing links keep working.

Styles are in `assets/css/site.css`, fonts in `assets/fonts/`, and the header artwork in `assets/img/`.

## Editing

- To change wording, edit the page's `index.html`.
- The header and menu are repeated in every page, so a menu change has to be made in each file.
- To add a blog post, copy one of the post folders, change its text, then add it to the lists in `blog/index.html` and `index.html`.

## Contact form

The form in `contact/index.html` does not send anywhere yet. Sign up with a form service that gives you a form address, then replace the `#` in `action="#"` with that address.

## Publishing

In the repository settings, under Pages, choose "Deploy from a branch", branch `main`, folder `/ (root)`.
