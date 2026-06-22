---
layout: default
title: Setup for Windows
---

# Setup for Windows

This page helps you prepare your Windows computer for Vibe Coding.

We use `winget` as a Package Manager. A Package Manager installs programs through commands in PowerShell. This may feel unfamiliar at first, but it is often easier than many separate download pages.

## What this page explains

You install and check:

- a GitHub account
- `winget`
- `Git`
- `Node.js LTS`
- `Zed`
- `OpenCode`
- a simple project folder

## Why this matters for Vibe Coding

A `Coding Agent` needs a place where it can work: a project folder with files.

For this workflow to work well, you need:

- an Editor to see and change files
- `Git` to save project states
- GitHub to store projects online
- `Node.js` so simple web projects can run later
- `OpenCode` so you can work with a Coding Agent inside the project

---

## Before you start

Open this page on your Windows computer and work through the steps from top to bottom.

If a step does not work: that is okay. Write down the error message or take a screenshot.

## Installation and setup

### 1. Create a GitHub account

`GitHub` is a website where you can store and share code. For this guide, a free personal account is enough.

1. Open [github.com](https://github.com/).
2. Click `Sign up`.
3. Create an account with your email address.
4. Confirm your email address.
5. Remember your username.

You do not need a paid plan.

### 2. Open PowerShell

`PowerShell` is a program where you run text commands.

1. Press the `Windows` key.
2. Type `PowerShell`.
3. Open `Windows PowerShell`.

You now see a window where you can type commands.

### 3. Check winget

`winget` is the Windows Package Manager. On Windows 11 and current Windows 10 versions, it is usually already installed.

Check in PowerShell:

```powershell
winget --version
```

If a version number appears, `winget` is ready.

If the command is not found:

1. Open the `Microsoft Store`.
2. Search for `App Installer`.
3. Install or update `App Installer`.
4. Close PowerShell and open it again.
5. Check again:

```powershell
winget --version
```

### 4. Install Git

`Git` saves versions of your project. This lets you understand later what changed.

Install `Git`:

```powershell
winget install --id Git.Git -e
```

Close PowerShell afterward and open it again.

Then check:

```powershell
git --version
```

If a version number appears, `Git` is installed.

### 5. Configure Git once

Git should know which name and email address belong to your changes.

Replace the example values with your own data:

```powershell
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Check afterward:

```powershell
git config --global user.name
git config --global user.email
```

If your name and email address are shown, it is set up correctly.

### 6. Install Node.js LTS

`Node.js` helps us later run simple web projects locally. `LTS` means: stable version for most users.

Install `Node.js LTS`:

```powershell
winget install --id OpenJS.NodeJS.LTS -e
```

Close PowerShell afterward and open it again.

Check the installation:

```powershell
node --version
npm --version
```

If both commands show a version number, everything is ready.

### 7. Install Zed

`Zed` is our Code Editor. You open and edit project files in it.

First check whether Zed is available through `winget`:

```powershell
winget search Zed
```

If you see an entry for `Zed`, install it. Usually the package name is:

```powershell
winget install --id Zed.Zed -e
```

If `winget` does not find a Zed entry, use the official download page:

1. Open [zed.dev/download](https://zed.dev/download).
2. Download Zed for Windows.
3. Start the installer.
4. Open `Zed` afterward.

### 8. Install OpenCode

`OpenCode` is the Coding Agent used in this guide. It runs in PowerShell.

Install OpenCode with `npm`:

```powershell
npm install -g opencode-ai
```

Check afterward:

```powershell
opencode --version
```

If a version number appears, OpenCode is installed.

### 9. Add OpenCode to Zed

OpenCode can run in Zed as an `External Agent`. Then you can chat with the Agent directly in Zed while your project folder is open.

Add OpenCode to Zed like this:

1. Open `Zed`.
2. Open your project or the folder `first-project`.
3. Open the Command Palette with `Ctrl + Shift + P`.
4. Search for `zed: acp registry`.
5. Open the ACP Registry.
6. Search for `OpenCode`.
7. Install the OpenCode Agent.
8. Open the Agent Panel through the sparkle icon or through the Command Palette with `agent: new thread`.
9. In the new Thread, choose `OpenCode` as the Agent.

If OpenCode asks you to sign in or connect, follow the instructions.

OpenCode needs access to an AI model. Depending on your setup, this can happen through an OpenCode account, an API key, or another provider.

If you are asked for an API key and do not have one yet, check the OpenCode documentation or the instructions from your AI provider.

You do not need to buy anything before you know which access you want to use.

Note: if you already happen to pay for another Coding Agent, for example `Codex`, `Claude Code`, `Copilot`, or another Agent in Zed, you can also use that. This guide uses OpenCode for the shared examples.

### 10. Test OpenCode in PowerShell

If the Zed connection does not work yet, you can also test OpenCode directly in PowerShell:

1. Open PowerShell.
2. Start OpenCode:

```powershell
opencode
```

### 11. Create a project folder

A project folder is simply a folder where all files of your project live.

Create a folder on the Desktop:

```powershell
cd Desktop
mkdir vibe-coding-projects
cd vibe-coding-projects
mkdir first-project
cd first-project
```

Check where you are:

```powershell
pwd
```

You should see a path that ends roughly like this:

```text
Desktop\vibe-coding-projects\first-project
```

### 12. Open the project in Zed

Open `Zed`.

Then:

1. Click `File`.
2. Click `Open Folder`.
3. Choose the folder `first-project`.
4. Open it.

You now see your project folder in Zed. It is still empty. That is normal.

---

## Short function test

Go to your project folder in PowerShell:

```powershell
cd Desktop\vibe-coding-projects\first-project
```

Start OpenCode:

```powershell
opencode
```

If OpenCode starts in PowerShell or can be selected as an Agent in Zed, you are ready to start.

If OpenCode does not start, check:

- Does `winget --version` output a version number?
- Does `node --version` output a version number?
- Does `npm --version` output a version number?
- Does `opencode --version` output a version number?
- Are you in the right folder?

## What you have learned

You prepared your Windows computer so you can work on your own project with a Coding Agent.

You also saw that a project does not start with code, but with a simple working environment: account, Package Manager, Editor, PowerShell, project folder, and Agent.
