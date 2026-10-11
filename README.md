# Albin Zeqiri — personal website

One-page site built with [Hugo](https://gohugo.io) and the [hugo-profile](https://github.com/gurusabarish/hugo-profile) theme (git submodule in `themes/hugo-profile` — don't edit files there; overrides live in `layouts/`).

## Preview locally

```sh
git submodule update --init   # first time only: fetch the theme
hugo server                   # http://localhost:1313
```

## Where things live

| What | Where |
| --- | --- |
| Hero, About, Recognition cards, Contact, social links | `hugo.yaml` |
| Papers (published + under submission / in progress) | `content/projects/<slug>.md` |
| News timeline | `data/news.yaml` |
| CV (hero button) | `static/cv_zeqiri.pdf` |
| Paper PDFs / images | `static/papers/`, `static/images/papers/` |
| Extra styling | `assets/css/custom.css` |

## Add a paper

Create `content/projects/<slug>.md`:

```yaml
---
title: "Paper title"
date: 2027-01-15
image: "/images/papers/my-teaser.png"     # card image
authors: ['Albin Zeqiri', 'Co-Author*', 'Enrico Rukzio']   # "Name*" = equal contribution
venue: "Proceedings of the 2027 CHI Conference on Human Factors in Computing Systems"
venue_short: "CHI '27"
tags: ["Experimental Study", "Quantitative Research"]
pdf: "/papers/my-paper.pdf"
doi: "https://doi.org/10.1145/..."
# under_submission: true   # or work_in_progress: true → listed in "Under Submission & In Progress"
# summary: "One sentence shown on the card."
---

{{< figure src="/images/papers/my-teaser.png" >}}

<h2>Abstract</h2>
Abstract text.
```

When an unpublished paper is accepted, remove `under_submission` / `work_in_progress` and add `venue`, `venue_short`, `pdf`, `doi`. BibTeX is generated automatically on the paper page.

## Add news

Copy a block in `data/news.yaml`. Items are sorted and grouped by year automatically; items dated in the future show an "Upcoming" badge.

## Deploy

`.github/workflows/deploy.yml` publishes to GitHub Pages on every push to `main` (Settings → Pages → Source: GitHub Actions). Set `baseURL` in `hugo.yaml` to the final URL.
