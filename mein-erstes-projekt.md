---
layout: default
title: My First Project
---

# My First Project: Poster Generator

## What this page explains

In this section, we build a small interactive `Poster Generator` together.

A `Poster Generator` is a simple website where you can change a digital poster: switch colors, try layouts, arrange shapes randomly, and edit text.

We are not building a perfect app. We are building a first working version so you understand the workflow with a `Coding Agent`:

1. describe the goal
2. set limits
3. check the plan
4. allow a small change
5. test the result
6. give feedback

## Why this matters for Vibe Coding

The Poster Generator is small enough for a first step, but large enough to practice real Vibe Coding.

You learn how to break a project into smaller parts. This matters because a `Coding Agent` produces better results when you do not give it everything at once.

You also practice setting clear limits:

- no external frameworks
- no database
- no login
- only `HTML`, `CSS`, and `JavaScript`
- plan first, then change files

That keeps you in control. The Agent writes code, but you decide what gets built and when the next step happens.

---

## Preparation

Before we start, you should have created your own `Repository` on GitHub.

A `Repository` is the project folder on GitHub. Later, it will contain your files, for example `index.html`, `style.css`, and `script.js`.

Open your Repository in `Zed` and start your `Coding Agent` there.

If you are not there yet, go back to the GitHub guide first.

## Project goal

At the end, you should have a small website that you can open in the browser.

| Part | Minimum goal |
| --- | --- |
| Poster area | A large visible area in the browser |
| Title text | Text displayed on the poster |
| Shapes | Abstract graphic elements |
| Color palettes | At least three selectable variants |
| Layouts | At least three different arrangements |
| `Randomize` | A button for new random compositions |

A screenshot is enough as the result. We do not need an export feature.

---

## Shared build process

### Step 1: Ask for a plan

Now we describe the project, but we do not allow file changes yet.

Copy this prompt:

```text
I want to build an interactive Poster Generator.

Use only HTML, CSS, and JavaScript.
Do not use external frameworks.
Do not build a database, login, or export feature.

The website should include:
- a large poster area
- title text
- abstract graphic shapes
- buttons for at least three color palettes
- buttons for at least three layout variants
- a Randomize button

First create a short plan in 3 to 5 steps.
Name exactly which files you would create or change.
Do not change any files yet.
```

Read the plan. It should look roughly like this:

- `index.html` for the structure
- `style.css` for styling and the poster area
- `script.js` for buttons and randomness

If the Agent wants to build more, for example a framework, database, or many new folders, stop it:

```text
Please keep it simpler.
Use only index.html, style.css, and script.js.
No frameworks and no additional tools.
```

### Step 2: Let the Agent build the first version

If the plan sounds reasonable, allow the first change.

Copy this prompt:

```text
The plan is okay.

Now create the first simple version.

Important:
- Use only HTML, CSS, and JavaScript.
- Keep the code easy to understand.
- Create only the files you named in the plan.
- First build only the basic version with poster area, title, shapes, and buttons.

Afterward, briefly explain:
1. Which files you created or changed.
2. How I can open the page in the browser.
3. What is not built yet.
```

### Step 3: Open the website in the browser

Now open the website so you can see the result.

If the Agent created a file called `index.html`:

1. Find `index.html` in the file tree on the left side of `Zed`.
2. Right-click `index.html`.
3. Choose an option like `Reveal in Finder`, `Show in Finder`, or `Show in Explorer`.
4. Then open the file in the browser with a double-click.

When your browser opens the file, the address bar usually shows a path that starts with `file://`. That is okay. It only means that you opened the file directly from your computer.

If your Agent started a local server, it will probably give you an address like this:

```text
http://localhost:3000
```

Copy this address into your browser.

`localhost` means: the website is currently running only on your own computer.

Check:

1. Can you see a poster area?
2. Are buttons visible?
3. Does something happen when you click the buttons?
4. Are there error messages?
5. Did the Agent build more than necessary without asking?

### Step 4: Give feedback

Now comes the most important part: you give concrete feedback.

Bad:

```text
Make it prettier.
```

Better:

```text
The poster still feels too empty.
Please add more abstract shapes.
Only change CSS and JavaScript.
The buttons and existing structure should stay the same.
```

Or:

```text
The layouts still look too similar.
Please create three clearly different layout variants:
1. a calm layout with lots of empty space
2. a dense layout with many shapes
3. a diagonal layout with strong movement

Only change what is necessary for that.
```

After every change, check the browser again.

### Step 5: Improve Randomize

When the basic version works, we improve the `Randomize` button.

Copy this prompt:

```text
Improve the Randomize button.

When someone clicks it, these things should change:
- positions of the shapes
- sizes of the shapes
- colors within the selected palette
- rotation of the shapes

The code should stay easy to understand.
Afterward, explain which function is responsible for the random composition.
```

Then check:

1. Does the poster visibly change?
2. Does the text stay readable?
3. Do the other buttons still work?

### Step 6: Optionally add motion

If there is time left, you can add a small animation.

Copy this prompt:

```text
Add a subtle animation.

The shapes may move slowly or pulse slightly.
There should be a button that turns motion on and off.

The animation should not distract from the text.
Keep the solution simple.
```

If the animation feels too busy, give direct feedback:

```text
The animation is too strong.
Please make it slower and reduce the movement.
The text should remain the focus.
```

### Step 7: Ask for a review

At the end, ask the Agent to review the project without changing anything directly.

Copy this prompt:

```text
Please review the Poster Generator.

Do not change any files.

Check:
- Are the controls understandable?
- Are the layouts really different?
- Does the code have unnecessary complexity?

Suggest only one next step.
```

Important: the Agent should only analyze here. You decide afterward whether anything else should change.

---

## Good closing question

Do not stop working immediately once something works.

Ask for a summary of the current state:

```text
Summarize:
1. What was built?
2. Which files were changed?
3. How do I test the project?
4. What would be the most useful next step?
5. Are there known problems or risks?
```

This summary helps you return to the project later.

## What you have learned

You built a first small browser project with a Coding Agent.

You practiced:

- describing a goal clearly
- setting technical limits
- asking for a plan first
- allowing changes in small steps
- checking results in the browser
- giving concrete feedback
- asking the Agent for a final review

This is the most important workflow for your own project: start small, check, improve, and stay in control.
