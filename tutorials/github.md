---
layout: default
title: GitHub Tutorial
---

# GitHub Tutorial

In this tutorial, you learn how to save your project with `Git` and `GitHub`.

We mainly work with the `Zed` interface, not with Terminal commands. The goal is: you should understand what is happening without having to memorize all Git commands right away.

## What this page explains

This page explains:

- what `Git` is
- what `GitHub` is
- why you should use both for Vibe Coding
- which terms matter
- how to create a Repository on GitHub
- how to bring it onto your computer with Zed
- how to add an existing project folder to a GitHub Repository
- how to save changes
- how to upload changes to GitHub

## Why this matters for Vibe Coding

When you work with a `Coding Agent`, many files can change quickly.

That is useful, but also risky. An Agent can:

- break something
- change too many files
- overwrite a good version
- make a solution more complicated than necessary

`Git` is your safety net. It saves project states. When something works, you can save that state. If something goes wrong later, you can see what changed.

---

## Git and GitHub in short

`Git` is a tool on your computer. It remembers changes in your project.

`GitHub` is a website where you can store your Git project online.

## The most important terms

### Repository

A `Repository`, or `Repo` for short, is a project folder managed by Git.

Example:

```text
my-first-project
```

If this folder is a Git Repository, Git can save changes inside it.

### Clone

`Clone` means: you copy a GitHub Repository to your computer. Then it is no longer only online; you also have a local copy.

Example:

```text
GitHub Repo online -> project folder on your laptop
```

After that, you can work on the files locally.

### Commit

A `Commit` is a saved project state.

A Commit needs a short message.

Good Commit messages:

```text
Add first homepage
```

```text
Change button colors
```

```text
Fix layout spacing
```

Bad Commit messages:

```text
asdf
```

```text
changes
```

```text
final final really final
```

### Stage

`Stage` means: you choose which changes should go into the next Commit.

Example:

- You changed `index.html`.
- You changed `style.css`.
- You want to save both changes.
- Then you stage both files and make a Commit afterward.

For the start: if you are working alone, you can usually stage all meaningful changes together.

### Push

`Push` means: you upload your local Commits to GitHub.

Example:

```text
Your laptop -> GitHub
```

Only after a Push is your new version visible online on GitHub.

### Pull

`Pull` means: you download new changes from GitHub to your computer.

Example:

```text
GitHub -> your laptop
```

If you work alone, you need `Pull` less often. Still, it is good to briefly check whether GitHub has new changes before you start working.

### Branch

A `Branch` is a separate line of development in Git.

For the beginning, stay on `main`. That is the main Branch.

Branches become important later when several people work on a project or when you want to try larger changes separately.

---

## The simple solo workflow

For the beginning, this workflow is enough:

1. Create a Repository on GitHub.
2. Clone the Repository to your computer with Zed.
3. Change files in Zed.
4. Check changes in the Git Panel.
5. Stage changes. (Which changes should really be saved?)
6. Create a Commit with a short message. (Save the current version on your computer.)
7. Push to GitHub. (Upload the version from your computer to GitHub.)

In short:

```text
Change -> Check -> Commit (Save) -> Push (Upload)
```

## Create and open a Repository

### 1. Create a new Repository on GitHub

1. Open [github.com](https://github.com/).
2. Sign in.
3. Click the `+` in the top right.
4. Choose `New repository`.
5. Give your Repository a name.

Example:

```text
my-first-vibe-coding-project
```

6. Choose `Public` or `Private`.
7. Activate `Add a README file`.
8. Click `Create repository`.

For your first projects, `Private` is completely fine. `Public` means other people can see your Repository.

### 2. Copy the Repository address

After creating it, you see your new Repository on GitHub.

1. Click the green `Code` button.
2. Choose `HTTPS`.
3. Copy the address.

It looks roughly like this:

```text
https://github.com/your-name/my-first-vibe-coding-project.git
```

This address tells Zed which Repository should be copied to your computer.

### 3. Clone the Repository in Zed

Open `Zed`.

Then:

1. Open the Command Palette.
   - macOS: `Cmd + Shift + P`
   - Windows: `Ctrl + Shift + P`
2. Search for `clone`.
3. Choose the Git clone action.
4. Paste the GitHub address.
5. Choose a place on your computer, for example your project folder.
6. Open the cloned project in Zed.

If Zed asks whether you want to sign in to GitHub, follow the login flow.

At the end, you should see your project in the file area on the left side of Zed.

### 3a. Add an existing project folder to GitHub

Sometimes you already have a project folder on your computer and want to put it under version control.

`Version control` means: Git starts tracking the files, so you can save project states as Commits and upload them to GitHub.

The beginner-safe way is:

1. Create a new Repository on GitHub.
2. Clone that Repository with Zed, as described above.
3. Open your old project folder in Finder or File Explorer.
4. Copy your project files into the cloned Repository folder.
5. Go back to Zed.
6. Check the Git Panel.
7. Stage the copied files.
8. Create a Commit, for example:

```text
Add existing project files
```

9. Push the Commit to GitHub.

Do not copy the hidden `.git` folder if your old project already has one. The `.git` folder contains Git history. Copying it into another Repository can confuse Git.

---

## Save your first change

### 4. Make the first change

Create a new file in Zed.

Name:

```text
index.md
```

Content:

```text
My first Vibe Coding project
```

Save the file.

Now your project has a change.

### 5. Open the Git Panel in Zed

The `Git Panel` shows which files were changed.

You can open it through:

- the Git icon in the status bar
- or the Command Palette with `git panel: toggle focus`

In the Git Panel, you should now see `index.md` as a changed or new file.

If you do not see anything, check:

- Is the file saved?
- Did you really open the cloned Repository?
- Are you in the right project folder?

### 6. Check the change

Before saving anything, look at the change.

In Zed, you can use the Git Panel or the `Project Diff` for that.

`Diff` means: Git shows you the difference between the old and the new state.

Example:

```text
Before: file does not exist.
After: index.md was added.
```

This matters because, especially in Vibe Coding, you should not blindly accept everything an Agent changed.

### 7. Stage the change

In the Git Panel, you can choose files that should go into the next Commit.

For the start:

1. Find `index.md` in the Git Panel.
2. Check the box next to the file.

Now the file is `staged`.

That means: this change will be saved in the next Commit.

### 8. Create a Commit

At the bottom of the Git Panel, there is a field for the Commit message.

Write:

```text
Add index.md
```

Then click the Commit button or use the keyboard shortcut Zed shows you.

Now you have created your first Commit.

That means: Git saved this project state.

### 9. Push the change to GitHub

The Commit is currently only on your computer.

To give it to GitHub, you have to `push`.

There is a `Push` button in the Git Panel. You can also search for `git: push` in the Command Palette.

After the Push:

1. Open your Repository on GitHub.
2. Reload the page.
3. Check whether `index.md` is visible there.

If yes: you successfully uploaded your local change to GitHub.

---

## Keep working and checking

### 10. Continue later

When you continue later, use this workflow:

1. Open the project in Zed.
2. Make a small change.
3. Check the change in the Git Panel.
4. Stage the right file.
5. Write a clear Commit message.
6. Commit.
7. Push.

Example:

```text
Change homepage text
```

Or:

```text
Add project cards
```

### 11. When to use pull

If you work alone, usually nothing happens on GitHub that did not first come from your computer.

Still, `Pull` is useful when:

- you worked on another computer
- you changed a file directly on GitHub
- other people work with you later

`Pull` brings changes from GitHub back to your computer.

In Zed, you find `Pull` in the Git Panel or through the Command Palette with `git: pull`.

---

### 12. Git and Coding Agents

When a Coding Agent changes files, look into the Git Panel afterward.

Ask yourself:

- Which files were changed?
- Do these changes match the task?
- Was something changed that was not necessary?
- Can I open or test the result?

Good prompt after an Agent change:

```text
Briefly summarize which files you changed and why.
Do not change anything else.
```

If everything fits, make a Commit.

Example:

```text
Add first prototype layout
```

### 13. Collaboration, briefly

Git and GitHub are also made for collaboration.

Several people can work on a project, share changes, and merge them later.

That is powerful, but it is also more complexity at the start. First, work alone on `main`.

Just remember: when you work with others later, `Pull`, `Branches`, and `Pull Requests` become more important.

## Mini glossary

| Term | Meaning |
| --- | --- |
| `Repository` | A project folder managed by Git |
| `Clone` | Copy a GitHub Repository to your computer |
| `Stage` | Select changes for the next Commit |
| `Commit` | Save a project state |
| `Push` | Upload local Commits to GitHub |
| `Pull` | Download new changes from GitHub |
| `Branch` | A separate line of development in Git |
| `main` | The main Branch of your project |
| `Diff` | A view that shows what changed |

---

## What you have learned

You now know what `Git` and `GitHub` are and why they matter for Vibe Coding.

You can create a Repository on GitHub, clone it to your computer with Zed, add existing project files, check changes, commit them, and push them to GitHub.

This is an important step: you now have a safety net for your projects.
