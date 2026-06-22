---
layout: default
title: Vibe-Coding Input
permalink: /theorie/
---

# Vibe-Coding Input

Vibe Coding means: you describe to a `Coding Agent` what you want to build, and you develop a working project together with it.

You do not write every line of code yourself. Your job is to formulate goals, make decisions, check results, and give good feedback. Of course, you can ask the AI for input when you do not understand something. What matters is that you stay in control so the result does not become generic "AI slop."

## What this page explains

This page explains the basic idea of `Vibe Coding`: how you work with a `Coding Agent`, which limits matter, and how you formulate good work requests.

## Why this matters for Vibe Coding

A Coding Agent can help you better when you can clearly name goals, context, limits, and check steps. This page gives you the most important rules for that.

---

## Contents

| Section | Topic |
| --- | --- |
| 1 | What Vibe Coding is |
| 2 | What Vibe Coding is good at |
| 3 | Where Vibe Coding is limited |
| 4 | The most important rule |
| 5 | Good prompts for starting |
| 6 | OpenCode in Zed |
| 7 | What you should always check |
| 8 | Good tasks for beginners |
| 9 | Errors as part of the workflow |
| 10 | Set limits |
| 11 | Use external references |
| 12 | `AGENTS.md` as project instructions |
| 13 | Advanced: AI Development Guide |
| 14 | Advanced: split the project into phases |
| 15 | Advanced: ask first, then build |
| 16 | Advanced: do not believe everything Agents say |
| 17 | Good closing question after every session |

---

## 1. What Vibe Coding is

Vibe Coding means working with a Coding Agent on a software project without having to write everything by hand yourself.

That can be very fast. It can also become chaotic if you:

- ask for too much at once
- do not check results
- do not ask what changed
- do not set limits for the Agent

In this guide, Vibe Coding does not mean: "The AI does everything."

It means: you use an Agent as a technical tool to try ideas faster, build prototypes, and support your own learning process.

## 2. What Vibe Coding is good at

Vibe Coding is especially strong for:

- quick prototypes
- small websites
- interactive sketches
- simple tools
- explanations of existing files
- translations of error messages
- small feature additions
- layout, text, structure, and styling
- breaking code into smaller steps
- comparing alternatives
- documentation and setup guides

A Coding Agent can read files, suggest changes, run code, and use error messages to keep working.

## 3. Where Vibe Coding is limited

Coding Agents make mistakes. They can sound convincing and still write wrong code.

Typical problems:

- The Agent builds more than you asked for.
- The Agent changes existing logic even though it is not necessary.
- The Agent invents libraries, functions, or APIs.
- The Agent misses side effects.
- The Agent makes code more complicated than necessary. (!)
- The Agent fixes a symptom, but not the real cause.
- The Agent can introduce security problems.
- The Agent can lose track in large projects.

That is why Vibe Coding only works well when you lead the process.

You do not have to understand every line of code. But you should always know:

- What should the project do?
- What was just changed?
- How can I test whether it works?
- What should the Agent do next?

## 4. The most important rule

Work in small steps.

Bad:

```text
Build me a complete interactive website with login, database, gallery, animations, and export feature.
```

Better:

```text
Create a simple homepage with a title, a short description, and a button.
Use only HTML and CSS.
Afterward, show me which files you changed.
```

When that works, the next step comes.

## 5. Good prompts for starting

A good prompt usually contains:

- goal
- context
- constraints
- desired result
- check step

Example:

```text
I want to build a small website for an interactive installation.
Create a simple HTML/CSS version with a title, a short intro text, and three project cards.
Do not use external frameworks.
Only change files in this folder.
Afterward, briefly explain what you changed and how I can open it in the browser.
```

It is even better if you ask for a plan first:

```text
I want to build a small website, but I barely know any code.
Please first suggest a short plan in 3 to 5 steps.
Do not change any files yet.
```

## 6. OpenCode in Zed

In this guide, the examples use `Zed` as the Code Editor and `OpenCode` as the Coding Agent.

A useful workflow:

1. Open your project in Zed.
2. Start OpenCode as an Agent in Zed.
3. Describe a small task.
4. Ask the Agent to explain the plan first.
5. Allow the change.
6. Check the result.
7. Give concrete feedback.

Example for the first prompt:

```text
Take a quick look at this project.
Explain in simple words which files are important for getting started.
Do not change anything yet.
```

Example for a small change:

```text
Create a very simple HTML page for a project called "My first Vibe Coding project".
It should have a title, a short description, and three colored sections.
Use only HTML and CSS.
Please change only the files necessary for this.
```

Example for feedback:

```text
This is too text-heavy.
Make the page more visual, but keep the existing structure.
Please only change the CSS.
```

## 7. What you should always check

After every change:

1. Which files were changed?
2. Can I start or open the project?
3. Does the result look roughly like what I wanted?
4. Are there error messages?
5. Did the Agent add extra things without asking?

If something is unclear, ask:

```text
Explain the last change in simple words.
Which file is most important?
Which lines should I look at?
```

## 8. Good tasks for beginners

Good first tasks are small, visible, and easy to check.

| Task | Why it fits well |
| --- | --- |
| Simple homepage | You quickly see a result in the browser |
| Small text or layout change | You can easily check the difference |
| Buttons without a database | You practice interaction without complex technology |
| README or project note | You learn to have files changed deliberately |
| Have an error explained | You understand problems before anything changes |

## 9. Errors are part of the workflow

If something does not work, do not blindly copy more prompts afterward.

Give the Agent the error message and the context.

Example:

```text
When starting, I get this error message:

[paste error message here]

Please first explain what it means.
Then suggest the smallest possible fix.
Do not change anything before you have explained the plan.
```

If the Agent already changed something and it got worse:

```text
The last change broke the layout.
Please analyze which change is probably responsible.
Suggest a minimal correction.
```

## 10. Set limits

Coding Agents work better when you set clear limits.

Useful constraints:

```text
Only change HTML and CSS.
```

```text
Do not add new dependencies.
```

```text
First create a plan and wait for my confirmation.
```

```text
Keep the solution as simple as possible.
```

```text
At the end, explain how I can test the result.
```

## 11. Use external references

For most tasks, a similar solution already exists. So we do not always have to write everything from scratch. We can give our Coding Agent a reference. This lets us build on a stable foundation and save time, energy, and tokens.

Examples:

- `three.js` demos
- CodePen examples
- GitHub repositories
- documentation
- screenshots of layouts
- small animation or interaction ideas

Important: a reference is not a finished work request.

Bad:

```text
Rebuild this Three.js demo for me.
```

Better:

```text
What I like about this Three.js demo is the slowly rotating 3D shape and the dark stage.
Please build a very simple own version of that.
Use only one sphere, one light source, and one camera.
First create a plan and tell me which files you would change.
```

When you use an external reference, describe:

- What exactly do you like about it?
- What should be adopted?
- What should not be adopted?
- How simple should the first version be?
- May the Agent use a library?

With libraries like `three.js`, this is especially important:

- Start with a small demo.
- Use the official documentation or a small example.
- Ask the Agent to explain which files are new.
- Test after every change in the browser.
- Do not ask for a complete 3D world in the first prompt.

Good prompt:

```text
I want to build a small Three.js scene as an experiment.
The scene should only show a rotating cube on a dark background.
Use the simplest possible structure.
First explain which files are needed.
Do not change anything before you have shown the plan.
```

## 12. AGENTS.md as project instructions

An `AGENTS.md` file is an instruction file for the Coding Agent.

It tells the Agent how it should work in a project. This is useful because Agents otherwise often guess which rules apply.

A good `AGENTS.md` can include:

- What is the goal of the project?
- Which files are important?
- How do you start the project?
- How do you test the project?
- Which design rules apply?
- Which files may the Agent change?
- Which files should the Agent not touch?
- How simple should the solution stay?
- When should the Agent ask first?

Example:

```md
# AGENTS.md

This project is a small prototype for an interactive installation.

## Workflow

- Make small, understandable changes.
- Explain your plan before larger changes.
- Do not add new libraries without asking.
- Do not change setup files unless it is really necessary.

## Testing

- Open `index.html` in the browser.
- Check whether text and buttons are visible.
- Check the browser console for errors.

## Design

- Keep the layout simple.
- Use clear contrast.
- No overloaded animations.
```

An `AGENTS.md` does not make the Agent perfect. But it reduces misunderstandings.

If your own project becomes larger, a small `AGENTS.md` is often better than one very long prompt.

## 13. Advanced: AI Development Guide

For larger projects, it is worth giving the Agent fixed project instructions.

That can be a file like:

- `AGENTS.md`
- `AI_DEVELOPMENT_GUIDE.md`
- `CONTRIBUTING.md`

For beginners, `AGENTS.md` is usually enough because many Coding Agents automatically pay attention to this file.

The most important content is not the perfect format, but clear rules:

- What are we building?
- What is currently not part of the project?
- Which commands test the project?
- What should stay simple?
- When must the Agent ask?

## 14. Advanced: split the project into phases

For larger projects, you should not build everything in one Thread.

Split the project into phases:

1. Concept
2. Basic structure
3. First visible version
4. Interaction
5. Styling
6. Tests
7. Cleanup
8. Documentation

For each phase, you can start a separate Agent Thread. This keeps the context cleaner and prevents old decisions from confusing the next step.

## 15. Advanced: ask first, then build

For larger changes, this prompt is useful:

```text
Please do not change anything yet.
First analyze the project and suggest a plan for the next change.
Name exactly which files you would change.
Then wait for my confirmation.
```

This gives you back control.

## 16. Advanced: do not believe everything Agents say

When an Agent makes a technical decision, ask for the reason:

```text
Why did you choose this solution?
Which simpler alternative would there be?
What are the disadvantages of your solution?
```

This matters especially for beginners because Agents often suggest overly complex solutions.

Simple code is usually better for the learning process.

## 17. Good closing question after every session

Do not end a Vibe Coding session just because something works.

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

## Short version

Vibe Coding is useful for quick prototypes and creative experiments. But it does not replace your judgment.

Work small, check often, set clear limits, and ask for changes to be explained. The larger the project becomes, the more important project rules, tests, Git, and clear phases become.

---

## What you have learned

You know the most important rules for working with Coding Agents: start small, set limits, check changes, and save good intermediate states.
