# Current differences with stock lb

| Element              | New Value                   | Line(s) Affected |
|----------------------|-----------------------------|:----------------:|
| Name                 | Benjamin Chausse            |         2        |
| Website              | https://chaussebenjamin.xyz |         4        |
| Editor               | nvim                        |         9        |
| Blog Post Titles     | `<h2></h2>`                 |        51        |
| Date Format          | `%z` -> `%Z`                |        47        |
| `link-bracket` class |                             |    49, 51, 69    |
| `post` class         |                             |      52, 66      |
| `post-author` class  |                             |        49        |
| `post-date` class    |                             |        51        |
| `post-link` class    |                             |      49, 51      |

| Class Name     | Applied to element:                                    | Affected File(s) |
|----------------|--------------------------------------------------------|------------------|
| `link-bracket` | `<small>` containing links related to individual posts | blog, standalone |
| `post`         | `<li>` referencing specific posts                      | blogindex        |
| `post-author`  | `<a>` for the author at the end of standalone posts    | standalone       |
| `post-date`    | `<small>` containing the date                          | blog             |
| `post-link`    | `<a>` for "link" and "Standalone" (in the `<small>`)   | blog, standalone |

## TODO
- [ ] Server-side "include header" for individual blog posts (for nginx)
- [ ] Change https://neovimer.xyz for https://chaussebenjamin.xyz once merger is complete
