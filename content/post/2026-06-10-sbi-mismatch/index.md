---
# ── Required Hugo fields ───────────────────────────────────────────────────────
title: "Your pill title here"
date: YYYY-MM-DD
lastmod: YYYY-MM-DD

# ── Authors — must match slugs in content/authors/ ────────────────────────────
authors:
  - your-author-slug

# ── Pill metadata (used by shortcodes) ────────────────────────────────────────
pill_type: "deep-dive"          # "deep-dive" or "survey"
pill_difficulty: "practitioner" # "beginner", "practitioner", or "researcher"
pill_reading_time: "12"         # estimated minutes, as a string

# For deep-dive only — remove these two lines for survey pills:
pill_paper: "Author et al., Year — Full paper title"
pill_paper_arxiv: "https://arxiv.org/abs/XXXX.XXXXX"

# ── Taxonomy ──────────────────────────────────────────────────────────────────
tags:
  - tag-one
  - tag-two
categories:
  - Pills

# ── Featured image (place as featured.png next to this file) ──────────────────
image:
  caption: ""
  focal_point: ""
  preview_only: false
---

<!-- PILL BODY — replace placeholder text with AI-generated content -->
<!-- Remove all HTML comments before publishing                      -->

{{< pill-badge type="deep-dive" >}}

{{< pill-meta
  difficulty="Practitioner"
  paper="Author et al., Year"
  code="Python examples included"
>}}

{{< pill-toc >}}

## The question {#the-question}

One paragraph. Plain language, no jargon. What problem does this paper (or
field) tackle, why does it matter, and to whom?

## Context & background {#context-background}

Four to five paragraphs. Historical arc, intellectual predecessors, what
was missing before this work.

<!-- Example figure — provide source image to AI, it generates the SVG -->
{{< pill-figure
  src="figures/figure1.svg"
  number="1"
  caption="Describe what the figure shows."
  source="Author et al., Year"
  arxiv="https://arxiv.org/abs/XXXX.XXXXX"
>}}

Continue with remaining paragraphs...

## Main contributions {#main-contributions}

<!-- For survey pills, rename this section to "Core concepts" and update
     the id to #core-concepts. The pill-toc shortcode reads pill_type
     from frontmatter and adjusts automatically. -->

Two to three paragraphs. The paper's central claims, methods, results.
Distinguish what is empirically shown vs. theoretically claimed vs. your
own interpretation.

{{< pill-callout >}}
**Key insight:** One sentence capturing the most important thing to
understand about this paper's contribution.
{{< /pill-callout >}}

## Intuition & worked example {#intuition-worked-example}

<!-- Deep-dive only. Remove this entire section for survey pills. -->

Jargon-free walkthrough. Concrete analogy first, then the mechanism, then
code.

```python
# Brief comment explaining what this demonstrates
# Minimal, self-contained Python — no heavy dependencies

import numpy as np

# Your example here
```

Prose continuing after the code block, explaining what the output means.

## Key papers {#key-papers}

{{< pill-papers >}}
| Paper | Authors | Year | Arxiv | Summary |
|-------|---------|------|-------|---------|
| Paper title one | A, B, C | 2020 | https://arxiv.org/abs/XXXX.XXXXX | One-line summary. |
| Paper title two | D, E | 2019 | https://arxiv.org/abs/XXXX.XXXXX | One-line summary. |
| Paper title three | F, G | 2021 | https://arxiv.org/abs/XXXX.XXXXX | One-line summary. |
| Paper title four | H | 2022 | https://arxiv.org/abs/XXXX.XXXXX | One-line summary. |
| Paper title five | I, J | 2023 | https://arxiv.org/abs/XXXX.XXXXX | One-line summary. |
{{< /pill-papers >}}

<!-- REMOVE BEFORE PUBLISHING -->
{{< pill-verification-note >}}
Replace this with the AI's verification output, e.g.:
- No dropped papers.
- ⚠️ Unverified: [paper name] — please confirm arxiv link before publishing.
- [citation needed] in section 3, paragraph 2, claim about X.
{{< /pill-verification-note >}}

## Open questions {#open-questions}

One to two paragraphs. What is genuinely unsolved. Failure modes. Where
consensus is weak. For deep-dives: limitations the authors themselves
acknowledge.

## Further reading {#further-reading}

One paragraph with 2–4 inline references and arxiv links. Written as
prose: "For a deeper treatment of X, [Paper A](link) is the clearest
entry point; [Paper B](link) extends this to Y..."

## Reader kit {#reader-kit}

{{< pill-reader-kit
  title="Your topic name"
  file="pill.md"
>}}
{{< /pill-reader-kit >}}
