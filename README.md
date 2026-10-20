# Folio

Folio is the official theme of the [`umono/blog@v0.1`](https://umono.dev/registry/v1/contracts/umono/blog/v0.1) contract for [Umono](https://github.com/umono-cms/umono). It is made for reading long articles: a paper-toned page, a serif designed for long-form text, a measure of about 66 characters and a generous line height.

| | |
| --- | --- |
| Theme ID | `umono/folio` |
| Contract | `umono/blog@v0.1` (`post`, `post-list` and `page` layouts) |
| Requires | Umono v0.9 or later |
| License | MIT, with the Literata font under the SIL Open Font License 1.1 ([LICENSE](LICENSE)) |

## Install

Download the `.umono-theme` file from the [latest release](https://github.com/umono-cms/theme-folio/releases/latest) and install it in your Umono project:

```sh
umono theme install umono_folio_0.1.0.umono-theme
```

Then activate it in the admin panel under **Settings → Themes**, and bind your pages to the layouts of `umono/blog v0.1`.

## Design

- **Type.** Text is set in [Literata](https://github.com/googlefonts/literata), a variable typeface made for reading on screens, with optical sizes for headings. The Latin and Latin Extended subsets are included, in `assets/fonts/`. Code is set in the system's monospace font.
- **Page.** A warm paper tone with dark brown ink. Body text is 17px on small screens and 19px from 48rem up, with a line height of 1.65.
- **Colors and sizes** are custom properties on the root in `assets/theme.css` (`--paper`, `--ink`, `--accent`, `--measure` and the rest).
- **Menu.** Submenus open on hover and on keyboard focus where the pointer can hover. On touch screens they are shown under their item.
- **Direction.** The theme uses logical properties and works in right-to-left languages.

`attributes.toml` gives the `post` and `post-list` layouts a root class (`folio-post`, `folio-post-list`) and sets `sizes` on the images of the `post` and `page` layouts.

## Development

```sh
umono theme dev     # live development at http://localhost:8990
umono theme build   # checks the theme and writes dist/umono_folio_<version>.umono-theme
```

See the [Umono CLI](https://github.com/umono-cms/cli) for the details of `dev` and `build`.
