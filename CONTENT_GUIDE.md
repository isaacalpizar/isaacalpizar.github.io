# Content Editing Guide

Quick reference for editing each section of the site.

---

## 1. Main Page (`/`)

**File:** `_pages/about.md`

| What | Field |
|---|---|
| Your subtitle/tagline | `subtitle:` |
| Profile photo | Replace `assets/img/prof_pic.jpg` |
| Circular vs. rounded photo | `image_circular: true/false` |
| Info below photo (office, email, etc.) | `more_info:` (supports HTML) |
| Show social icons in navbar | `social: true/false` |
| Show news section | `announcements.enabled: true/false` |
| Number of news items shown | `announcements.limit:` |
| Body text (bio) | The markdown content below the `---` |

**Also:** `_config.yml` controls your name (`first_name`, `last_name`), site keywords, and which social icons appear (see `_data/socials.yml`).

**Social icons:** `_data/socials.yml` — uncomment and fill in any service (email, LinkedIn, ORCID, Google Scholar, etc.).

---

## 2. News

**Folder:** `_news/`

Each file is one news item. Create a new `.md` file (any filename) with:

```yaml
---
layout: post
date: 2026-04-17 10:00:00
inline: true
---

Your news text here. Supports **markdown** and [links](https://example.com).
```

- `inline: true` — shows text directly on the main page (recommended for short items)
- `inline: false` — adds a "read more" link to a separate page
- Items are sorted by `date`, newest first
- The main page shows the latest 3 (controlled by `announcements.limit` in `_pages/about.md`)

---

## 3. Blog

**Folder:** `_posts/`

Filename format is **required**: `YYYY-MM-DD-your-title.md`

```yaml
---
layout: post
title: My Post Title
date: 2026-04-17 12:00:00
description: Short description shown in the blog listing
tags: tag1 tag2
categories: category-name
featured: false   # set true to pin to top
---

Post content in markdown.
```

- `tags` and `categories` are space-separated
- Images go in `assets/img/` and are referenced as `assets/img/your_image.jpg`
- Featured posts appear at the top of the blog listing

---

## 4. Selected Publications

**File:** `_bibliography/papers.bib`

Add a standard BibTeX entry. To make it appear on the **selected publications** page, add `selected={true}`:

```bibtex
@article{yourkey2026,
  title        = {Your Paper Title},
  author       = {Alpizar-Chacon, Isaac and Co-Author, Name},
  journal      = {Journal Name},
  year         = {2026},
  selected     = {true},       % shows on /publications/
  abbr         = {JN},         % badge label (optional)
  pdf          = {paper.pdf},  % file in assets/pdf/ (optional)
  html         = {https://doi.org/...},  % DOI link (optional)
  abstract     = {Your abstract here.},  % (optional)
  code         = {https://github.com/...},  % (optional)
}
```

**Key optional fields:**

| Field | Effect |
|---|---|
| `selected={true}` | Appears on /publications/ page |
| `abbr={XX}` | Colored badge next to title |
| `pdf={file.pdf}` | PDF button (place file in `assets/pdf/`) |
| `html={url}` | Link button |
| `code={url}` | Code button |
| `abstract={...}` | Expandable abstract |
| `preview={image.jpg}` | Thumbnail (place in `assets/img/`) |

Scholar name matching is set in `_config.yml` under `scholar.last_name` / `scholar.first_name` — your name is bolded automatically.

---

## 5. Projects

**Folder:** `_projects/`

Create a new `.md` file (any filename) for each project:

```yaml
---
layout: page
title: Project Title
description: One-line description shown on the card
img: assets/img/your_image.jpg   # card thumbnail (optional)
importance: 1                     # lower number = appears first within category
category: current                 # "current" or "past"
---

Full project description in markdown.
```

- `category: current` → appears under the **current** section
- `category: past` → appears under the **past** section
- `importance` controls order within each category (1 = first)
- The page layout (`layout: page`) gives you a full project detail page with its own URL

---

## 6. Teaching

**Folder:** `_teachings/`

Create a new `.md` file for each course:

```yaml
---
layout: course
title: Course Title
description: Short description
year: 2026
term: Spring          # Spring, Fall, Summer, etc.
instructor: Prof. Isaac Alpizar-Chacon
location: Room 101
time: Tuesdays 10:00–12:00
course_id: unique-course-id
schedule:
  - week: 1
    date: Feb 3
    topic: Introduction
    description: Overview of the course.
    materials:
      - name: Slides
        url: /assets/pdf/slides.pdf
      - name: Assignment 1
        url: /assets/pdf/assignment1.pdf
---

## Course Overview

Description, prerequisites, grading, etc. in markdown.
```

**Also edit:** `_pages/teaching.md` to update the page description shown at the top of `/teaching/`.
