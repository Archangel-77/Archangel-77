# CV package

Three artefacts, each for a different reader.

| File | For | Why it exists |
|---|---|---|
| `index.html` | Humans | One self-contained file, no build step, no external assets. Prints to a designed A4 PDF. |
| `cv.txt` | Automated parsers | Plain ASCII for ATS ingestion and LLM-based screening, with no layout to mangle. |
| `../generate_resume.py` | Application portals | The ATS-safe DOCX/PDF. Single column, standard section names, no tables. |

## Why the HTML embeds structured data

`index.html` carries a JSON-LD `Person` schema in its `<head>`. Most screening
pipelines now parse a CV with a language model before a human sees it, and a
plain PDF gives that model nothing but positional text. The schema states name,
title, contact, location, credentials, and `knowsAbout` explicitly, so the
machine reads the same facts a person does.

Verify it with Google's Rich Results Test, or:

```bash
curl -s https://archangel-77.github.io/Archangel-77/cv/ | grep -A2 'application/ld+json'
```

## Print to PDF

Open `cv/index.html` in a browser and use the **Print / Save as PDF** button, or:

- **Chrome / Edge** — Ctrl+P, destination *Save as PDF*, paper **A4**,
  margins **Default**, and tick **Background graphics** off.
- **Firefox** — Ctrl+P, then *Print to File*.

The stylesheet sets `@page { size: A4 }` and keeps entries from splitting across
pages, so the output is stable. It is designed to land on two pages.

## Publish to GitHub Pages

The profile repository is `Archangel-77/Archangel-77`.

> **On the URL path:** a repository named the same as its owner is the *profile* repo,
> not the `<owner>.github.io` root repo. GitHub therefore serves it under the
> repository name rather than at the domain root.

Pages is already enabled for this repository (branch `main`, folder `/`), so the CV is
live at:

**https://archangel-77.github.io/Archangel-77/cv/**

To re-enable it or point it elsewhere:

```bash
gh api -X POST repos/Archangel-77/Archangel-77/pages \
  -f 'source[branch]=main' -f 'source[path]=/'
```

That URL is worth more than the CV itself: it is clickable from your GitHub
profile, your email signature, and a LinkedIn headline.

## Keeping it current

The CV and `generate_resume.py` describe the same facts and will drift. When
something changes — a release, a new project, a finished contract — update both
in the same sitting. The numbers on this CV are deliberately limited to ones a
reader can verify:

- `feedstream.fly.dev` returns 200
- `conductor-task-queue` is on PyPI at the stated version
- the release count is visible on the Hutsix releases page
- the ADR count is visible in `feedstream/docs/adr/`

Do not add a metric that cannot be traced to a public artefact. A recruiter
cannot disprove an invented percentage, but an engineer across the table can,
and that is the only conversation that matters.
