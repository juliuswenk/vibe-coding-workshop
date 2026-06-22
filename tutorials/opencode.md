---
layout: default
title: OpenCode Tutorial
---

# OpenCode Tutorial

In this tutorial, you learn how to use `OpenCode` in `Zed`.

OpenCode is a `Coding Agent`: you give it tasks, questions, and feedback. The Agent can read your project, suggest changes, and help build your project.

## What this page explains

This page explains:

- what OpenCode is
- how OpenCode is integrated into Zed
- what the Agent Panel is
- what Threads are
- how to start an OpenCode Thread
- which options matter
- how to choose a model
- how to give the Agent good context
- how to check changes
- when to start a new Thread

## Why this matters for Vibe Coding

When you use OpenCode in Zed, you work directly inside the project. That means:

- The Agent can see your files.
- You can check changes directly.
- You can use Git to save good intermediate states.
- You can keep working in small steps.

---

## What is OpenCode?

`OpenCode` is a Coding Agent.

A Coding Agent is more than a chatbot. It can work with your project:

- read files
- explain code
- plan changes
- change files
- analyze error messages
- suggest or run commands if you allow it

Important: OpenCode is a tool. It does not replace your own thinking.

---

## Install OpenCode in Zed

Zed can install external Agents through the `ACP Registry`.

`ACP` stands for `Agent Client Protocol`. For you, this simply means: Zed can integrate OpenCode as an external Agent.

Install OpenCode in Zed like this:

1. Open `Zed`.
2. Open the Command Palette.
   - macOS: `Cmd + Shift + P`
   - Windows: `Ctrl + Shift + P`
3. Search for:

```text
zed: acp registry
```

4. Open the ACP Registry.
5. Search for `OpenCode`.
6. Install OpenCode.
7. Restart Zed if Zed asks you to.

Why do this?

After installation, OpenCode can be used directly in Zed's Agent Panel. You do not have to constantly switch between the Editor and an external Terminal.

---

## Open the Agent Panel

The `Agent Panel` is the area in Zed where you work with an Agent.

Open it through:

- the sparkle icon in Zed
- or the Command Palette with:

```text
agent: new thread
```

Why do this?

The Agent Panel keeps your conversation with the Agent directly next to your project. You can ask questions and see which files are affected at the same time.

## Start an OpenCode Thread

A `Thread` is a conversation with an Agent.

Start an OpenCode Thread like this:

1. Open the Agent Panel.
2. Open the menu for a new Thread.
3. Choose `OpenCode` as the Agent.
4. Write your first prompt.

Good first prompt:

```text
Take a quick look at this project.
Explain in simple words which files are important.
Do not change anything yet.
```

Why do this?

You first give the Agent an analysis task instead of a build task. This helps you better understand what you are working with.

---

## Choose a model

OpenCode needs an AI model in the background.

Depending on the OpenCode configuration, you can choose a model.

Typical differences between models:

- Some models are faster.
- Some models are better at complex tasks.
- Some models can handle longer context better.
- Some models give better explanations.

For beginners:

Why does this matter?

The model choice affects quality, speed, and sometimes cost. At the start, clean work is more important than immediately finding the "best" model.

## Thread Panel and Thread History

Zed can manage several Agent Threads.

A Thread is useful for one concrete task.

Examples:

```text
Thread 1: Understand project
Thread 2: Build homepage
Thread 3: Improve layout
Thread 4: Fix error
```

Why do this?

Separate Threads keep the context cleaner. If a Thread becomes very long, the Agent can mix up old decisions.

For beginners, this is enough:

- Use one Thread per larger work step.
- Start a new Thread when the topic changes.
- Ask for a summary at the end of a Thread.

Good closing prompt:

```text
Summarize:
1. What was built?
2. Which files were changed?
3. How do I test the project?
4. What is the next useful step?
```

---

## Mention files

If you know which file matters, name it directly.

Example:

```text
Look at `index.html` and `style.css`.
Explain how the page is structured.
Do not change anything yet.
```

Why do this?

The Agent focuses on the relevant files and wastes less time on the rest of the project.

## Tool permissions and confirmation

A Coding Agent can use tools depending on its settings, for example changing files or running commands.

If Zed or OpenCode asks whether an action is allowed, briefly read what is supposed to happen.

Pay special attention to:

- Which file is being changed?
- Is a command being run?
- Are new packages being installed?
- Are many files being changed?

Why do this?

You avoid letting the Agent do too much at once.

Good limit:

```text
Do not add new libraries without asking first.
```

---

## When to start a new Thread

Start a new Thread when:

- a topic is finished
- the Thread has become very long
- the Agent keeps going in circles
- you begin a new task
- you want a clean summary as the starting point

Good start for a new Thread:

```text
Here is the current state:
[paste short summary]

Please suggest the next small step.
Do not change anything yet.
```

Why do this?

A new Thread reduces old baggage. That helps the Agent work with more focus.

## Good first prompts

Understand project:

```text
Look at this project.
Explain in simple words which files are important.
Do not change anything.
```

Create plan:

```text
I want to build a simple project page.
Please first suggest a plan in 3 to 5 steps.
Do not change any files yet.
```

Small change:

```text
Create a simple homepage with a title, short description, and three cards.
Use only HTML and CSS.
Only change the necessary files.
Afterward, explain what you changed.
```

Explain error:

```text
I get this error message:

[paste error message]

Please explain it in simple words.
Suggest the smallest possible fix.
Do not change anything yet.
```

## What you have learned

You now know how OpenCode is integrated into Zed and how to start an OpenCode Thread.

You know the most important options: Agent Panel, Threads, model choice, auth, context, tool confirmations, and Git checks.

The most important point: let OpenCode start small, check every change, and save good intermediate states with Git.
