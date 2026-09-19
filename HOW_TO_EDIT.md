# Updating the CARAVEL website

The site is built with Jekyll and published from this repository. Edit a file
on GitHub (or locally), commit, and the site updates in a few minutes.

- Home page content (papers, team, banner, contacts, ...): [`index.md`](index.md)
- News articles: one file per article in [`_news/`](_news/)
- Images: [`assets/img/`](assets/img/)

> In `index.md`, indentation matters (YAML). Copy an existing block and change
> only the text inside the quotes.

---

## Add a paper

In `index.md`, under `# Publications Section`, copy a block and paste it at the
top of the list (newest first):

```yaml
    - date: "Mar 2026"
      type: "conference"        # journal | conference | preprint
      tag: "Conference"         # label on the card
      title: "Title of the paper"
      venue: "Journal or conference name"
      url: "https://link-to-the-paper"
      github: "https://github.com/..."   # optional, adds a "Code" button
```

## Add a team member

In `index.md`, under `# Team Section` → `members:`, copy a block:

```yaml
    - name: "Name Surname"
      photo: "/assets/img/team/name-surname.jpeg"   # optional
      role: "PhD Student at EURECOM"
      website: "https://..."
      linkedin: "https://..."
      scholar: "https://..."
```

- Delete any link line that does not apply (the icon then disappears).
- Without `photo`, a grey placeholder circle is shown.
- Upload photos (square, `.jpeg`) to `assets/img/team/`.
- To remove a person, delete their block.

The "open positions" button (`cta` → `url` in the Team Section) can point to
a web page (`"https://..."`) or to an email address (`"mailto:name@eurecom.fr"`).

## Add a news article

Create a new file in `_news/`, e.g. `_news/my-news-title.md`:

```markdown
---
title: "Title of the news"
date: 2026-09-30
category: "Publication"
excerpt: "One short sentence shown on the card."
image: /assets/img/news/my-image.png
---
Article text in Markdown.
```

- The 3 most recent news items appear on the home page; all appear on `/news/`.
- Upload the image to `assets/img/news/` first.
- The article URL is `/news/<file-name-without-.md>/`.

## Top banner

In `index.md`, under `# Banner Section`: edit `text` and `link.url`, or set
`enable: false` to hide it.

## Other sections

All in `index.md`; search for the section comment:

| Content                         | Section comment                |
| ------------------------------- | ------------------------------ |
| Title and subtitle              | `# Hero Section`               |
| Funder / partner logos          | `# Partners / Funding Section` |
| Research topics                 | `# Research Section`           |
| Group leader, open positions    | `# Team Section`               |
| Address, email, institution     | `# Contacts Section`           |


## Links inside a text

In `index.md` texts (e.g. the `bio` of the group leader), a link is written as:

```yaml
bio: "Professor at <a href=\"https://www.eurecom.fr\">EURECOM</a>."
```

Replace the URL and the visible text (`EURECOM`). Inside the quotes, each `"`
of the link must be written as `\"`. In `_news/` articles, use Markdown
instead: `[EURECOM](https://www.eurecom.fr)`.

## Troubleshooting

If the site does not update, the most likely cause is a YAML error (missing
quote, wrong indentation) or a malformed news header (the two `---` lines).
Check the **Actions** tab for the build log, or revert the last commit.

To preview locally: `bundle exec jekyll serve --livereload`.
