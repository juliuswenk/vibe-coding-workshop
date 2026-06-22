---
layout: default
title: Zed Tutorial
---

# Zed Tutorial

In this tutorial, you learn what `Zed` is and how to find your way around its interface.

Zed is the program where you open and edit your project files, work with Git, and later use your Coding Agent.

## What this page explains

This page explains:

- what a Code Editor is
- why Zed is useful for this workflow
- how Zed is roughly structured
- which parts of the interface matter
- how to open a project
- how to create and edit files
- where to find Git and Agent features

## Why this matters for Vibe Coding

When Vibe Coding, you do not only work in a chat window.

You need an environment where you can:

- see files
- check changes
- edit code or text
- start or test your project
- save with Git
- work with a Coding Agent inside the project

Zed is this working environment. If you roughly understand Zed, you can better follow what an Agent changes in your project.

---

## What is a Code Editor?

A `Code Editor` is a program for editing code and text files.

You can think of it as a very specialized text editor.

A normal text editor can write text. A Code Editor can also:

- show project folders
- highlight code with colors
- make errors visible
- search files quickly
- show Git changes
- open a terminal
- connect to Coding Agents

Examples of Code Editors are:

- `Zed`
- `Visual Studio Code`
- `Sublime Text`
- `Atom`

---

## The most important areas in Zed

Zed roughly consists of these areas:

```text
Project files on the left | Editor in the middle | Panels at the bottom/side
```

Depending on window size or settings, panels may appear in different places. That is normal.

### 1. Project Panel

The `Project Panel` shows the files and folders of your project.

Typical things you do there:

- open files
- create new files
- create folders
- rename files
- see which files belong to the project

Example:

```text
my-project
├── index.html
├── style.css
└── README.md
```

When you click a file, it opens in the Editor.

### 2. Editor area

The Editor is the large area in the middle.

This is where you edit files.

Zed highlights code with colors. This is called `Syntax Highlighting`.

It helps you recognize:

- What is text?
- What is an HTML tag?
- What is a filename?
- What might be an error?

### 3. Tabs

When you open several files, they appear as Tabs.

Example:

```text
index.html | style.css | README.md
```

A Tab is like an open browser tab.

You can switch between files without searching for them every time.

### 4. Command Palette

The `Command Palette` is a search function for Zed commands.

Open it with:

- macOS: `Cmd + Shift + P`
- Windows: `Ctrl + Shift + P`

Then you can search for actions.

Examples:

```text
git panel
```

```text
agent: new thread
```

```text
zed: acp registry
```

If you do not know where a feature is, the Command Palette is often the fastest way.

### 5. Terminal

The `Terminal` is an area where you can run text commands.

In Zed, you can open a Terminal directly inside the project.

That is useful because you do not have to switch between many windows.

Examples of commands:

```text
node --version
```

```text
opencode --version
```

```text
git status
```

You do not need to know many commands at the start. But you should know that the Terminal exists.

### 6. Git Panel

The `Git Panel` shows which files have changed.

You use it to:

- look at changes
- stage files
- create commits
- push changes to GitHub
- pull changes from GitHub

This is especially important in Vibe Coding because a Coding Agent can change several files.

After Agent changes, you should always briefly look at the Git Panel.

Ask yourself:

- Which files were changed?
- Does that match the task?
- Was anything unexpected changed?

### 7. Agent Panel

The `Agent Panel` is the area where you work with a Coding Agent.

There you can, for example:

- ask questions about your project
- have files explained
- ask for small changes to be planned
- have changes made
- have error messages explained

Good first prompt:

```text
Take a quick look at this project.
Explain in simple words which files are important.
Do not change anything yet.
```

Important: do not let the Agent build everything immediately. Start small.

---

## Working with a project

### 8. Open a project

A project is usually just a folder.

To open a project in Zed:

1. Open `Zed`.
2. Click `File`.
3. Choose `Open Folder`.
4. Select your project folder.
5. Open it.

After that, the folder should be visible on the left in the Project Panel.

### 9. Create a file

In the Project Panel:

1. Right-click your project folder.
2. Choose `New File`.
3. Enter a filename.

Example:

```text
index.html
```

Then you can edit the file in the Editor.

### 10. Typical workflow in Zed

For the beginning, this workflow is enough:

1. Open the project folder in Zed.
2. Briefly look at which files exist.
3. Ask the Coding Agent for a small plan.
4. Let it make a small change.
5. Check the result.
6. Open the Git Panel.
7. Look at the changes.
8. Create a commit if it works.

In short:

```text
Open -> Plan -> Change -> Check -> Commit
```

---

## Stay oriented

### 11. What you do not have to understand immediately

At the beginning, you do not have to understand:

- all settings
- all keyboard shortcuts
- debugging
- worktrees
- complex Git features
- all Agent profiles
- every error message

That comes later when you actually need it.

For the start, it is enough to:

- open a project
- find files
- edit files
- open the Git Panel
- open the Agent Panel
- check small changes

### 12. If you get lost

If Zed becomes confusing:

1. Close unnecessary Tabs.
2. Reopen the project folder.
3. Search files with `Cmd + P` or `Ctrl + P`.
4. Open the Command Palette and search for the feature.
5. Ask the Coding Agent:

```text
I am unsure where I am in Zed right now.
Explain which file I should open and why.
Do not change anything.
```

## What you have learned

You now know what Zed is, roughly what an IDE means, and which interface areas are important for Vibe Coding.

You can open a project, find files, create new files, find the Git Panel, and understand what the Agent Panel is for.

That is enough to not only write prompts, but to really work on your own project.
