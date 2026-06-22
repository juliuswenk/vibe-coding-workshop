# AGENTS.md

This repo contains the student-facing website for the Vibe Coding Workshop at SRH.
All changes should help students without coding, Git, or Terminal experience follow the workshop safely.

## Website

- The website is built with GitHub Pages.
- The default theme is `jekyll-theme-minimal`.
- Keep the two-column Minimal Theme structure: navigation/meta on the left, content on the right.
- No custom frontend app, no React/Vite/Next, no unnecessary JavaScript as long as Markdown and Jekyll are enough.
- Only touch styling when explicitly requested or when it clearly improves readability.
- If styling changes, prefer small changes: colors, spacing, typography, navigation.
- The website replaces slides. Do not plan a slide structure unless explicitly requested.

## Target audience

- Students have probably never worked with Git, GitHub, Terminal, or code before.
- Terms must be introduced slowly.
- Every guide should be understandable without prior knowledge.
- Do not assume shorthand like "clone the repo", "make a commit", or "install a dependency" without briefly explaining it.
- Vibe Coding should be taught as a tool, not as a magical complete solution.
- The important parts are concepts, good problem breakdown, and iterative work with Coding Agents.

## Language and tone

- Student-facing content is in English.
- Established English technical terms stay in English, for example `Prompt`, `Coding Agent`, `Repository`, `Commit`, `Branch`, `Markdown`, `Vibe Coding`.
- Briefly explain an important term the first time it appears.
- Tone: clear, calm, guiding, and lightly encouraging.
- No academic distance, but also no marketing tone.
- Occasionally point out what students have already accomplished.

## Page structure

- One Markdown file per topic.
- Use short, stable filenames in kebab-case.
- Split pages so students can quickly find the right place during the workshop.
- Avoid long collection pages when several independent steps emerge.
- Set internal links between related pages.

Planned structure:

```text
index.md
theorie.md
setup/
  mac.md
  windows.md
tutorials/
  github.md
  zed.md
  coding-agent.md
mein-erstes-projekt.md
freies-projekt-inspiration.md
glossar.md
knowledge-base.md
```

The structure may be adjusted if that makes the workshop easier to use.

## Required structure for each content page

Every student-facing `.md` file should contain these three orientation parts:

1. At the beginning: `## What this page explains`
   - Briefly state what the page is about.
   - Use at most a few paragraphs or a short list.

2. After that: `## Why this matters for Vibe Coding`
   - Explain the benefit of this part for working with Coding Agents.
   - Stay practical: what can students decide, prepare, or execute better afterward?

3. At the end: `## What you have learned`
   - Briefly summarize what students can do or understand after this section.
   - It may be encouraging, but should stay concrete.

Example:

```md
## What this page explains

This page shows you how to ...

## Why this matters for Vibe Coding

A Coding Agent can help better when ...

...

## What you have learned

You have now ...
```

## Writing rules for guides

- Number steps when they must happen in a fixed order.
- Use short paragraphs.
- Put code, filenames, commands, and technical terms in backticks.
- No long theory blocks without concrete application.
- For commands, briefly say where they are run.
- Anticipate likely beginner mistakes.
- Screenshots or simple visualizations are welcome when they genuinely help students.
- Visual flavor is allowed: small diagrams, icons, screenshots, sketches, or simple callouts.
- Visual elements must not make the page harder to maintain.

## Workshop philosophy

- Simplicity wins.
- Markdown before custom code.
- Existing Jekyll/GitHub Pages features before custom logic.
- Do not build features "for later."
- Do not hard-code tooling assumptions in `AGENTS.md`, because workshop tools may change.
- Content must be usable during a 4-hour workshop: quickly findable, clearly structured, not overloaded.

## What does not belong in this repo

- Complex web app structures.
- Unnecessary build tools.
- Unrequested design systems.
- Long presentation slides as a replacement for the website.
- Sample solutions outside the explicitly intended area.

## Check before finishing

- Link new or changed pages in the GitHub Pages structure.
- Check whether beginners can understand the terms.
- Check whether every content page contains the three required parts.
- Check whether the two-column Minimal Theme structure is preserved.
- For larger pages, build locally or at least carefully check the Markdown structure.
