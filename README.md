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
| Post: Why the name Life Reconnect | `2026/06/23/why-the-name-life-reconnect/index.html` |
| Post: Legacy work | `2026/01/12/legacy-work/index.html` |

The main pages keep the addresses they had on the old WordPress site. The two posts were re-dated to 2026; the `2020/` folders hold small redirect pages so links to the old post addresses still arrive.

Styles are in `assets/css/site.css`, fonts in `assets/fonts/`, and the header artwork in `assets/img/`.

## Editing

- To change wording, edit the page's `index.html`.
- The header and menu are repeated in every page, so a menu change has to be made in each file.
- To add a blog post, copy one of the post folders, change its text, then add it to the lists in `blog/index.html` and `index.html`.

## Contact form

The form in `contact/index.html` emails each message through FormSubmit (formsubmit.co). The delivery address is set in the `endpoint()` function in the script at the bottom of that file.

- The first message sent from the live site makes FormSubmit email an activation link to the delivery address. Messages are only delivered after that link is clicked.
- The activation email also gives a random code that can replace the address in `endpoint()`, which keeps the address out of the page entirely.
- Visitors answer a simple sum before the form sends, and a hidden trap field discards automated submissions.

## Publishing

In the repository settings, under Pages, choose "Deploy from a branch", branch `main`, folder `/ (root)`.
