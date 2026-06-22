---
layout: default
title: Setup for macOS
---

# Setup for macOS

This page helps you prepare your Mac for the workshop.

We use `Homebrew` as a Package Manager. A Package Manager installs programs through commands in the Terminal. This may feel unfamiliar at first, but it is often easier than many separate download pages.

## What this page explains

You install and check:

- a GitHub account
- `Homebrew`
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

Open this page on your Mac and work through the steps from top to bottom.

If a step does not work: that is okay. Write down the error message or take a screenshot.

## Installation and setup

### 1. Create a GitHub account

`GitHub` is a website where you can store and share code. For the workshop, you need a free personal account.

1. Open [github.com](https://github.com/).
2. Click `Sign up`.
3. Create an account with your email address.
4. Confirm your email address.
5. Remember your username.

You do not need a paid plan.

### 2. Open Terminal

The `Terminal` is a program where you run text commands.

1. Press `Cmd + Space`.
2. Type `Terminal`.
3. Press `Enter`.

You now see a window where you can type commands.

### 3. Install Homebrew

`Homebrew` installs programs on your Mac.

Copy this command into the Terminal and press `Enter`:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

The installer explains what it is doing. If it asks for your password: type your Mac password and press `Enter`.

Important: while typing the password, you do not see any characters. That is normal.

If Homebrew shows `Next steps` at the end, run those commands too. Then close Terminal and open it again.

Check afterward:

```sh
brew --version
```

If a version number appears, `Homebrew` is installed.

### 4. Install Git

`Git` saves versions of your project. This lets you understand later what changed.

Install `Git`:

```sh
brew install git
```

Check afterward:

```sh
git --version
```

If a version number appears, `Git` is installed.

### 5. Configure Git once

Git should know which name and email address belong to your changes.

Replace the example values with your own data:

```sh
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Check afterward:

```sh
git config --global user.name
git config --global user.email
```

If your name and email address are shown, it is set up correctly.

### 6. Install Node.js LTS

`Node.js` helps us later run simple web projects locally. `LTS` means: stable version for most users.

Install `Node.js`:

```sh
brew install node
```

Check afterward:

```sh
node --version
npm --version
```

If both commands show a version number, everything is ready.

### 7. Install Zed

`Zed` is our Code Editor. You open and edit project files in it.

Install `Zed`:

```sh
brew install --cask zed
```

Then start `Zed` from the Applications folder or through Spotlight:

1. Press `Cmd + Space`.
2. Type `Zed`.
3. Press `Enter`.

### 8. Install OpenCode

`OpenCode` is the Coding Agent we want to use in the workshop. It runs in the Terminal.

Install `OpenCode`:

```sh
brew install anomalyco/tap/opencode
```

Check afterward:

```sh
opencode --version
```

If a version number appears, OpenCode is installed.

If that does not work, use the `npm` variant:

```sh
npm install -g opencode-ai
```

### 9. Add OpenCode to Zed

OpenCode can run in Zed as an `External Agent`. Then you can chat with the Agent directly in Zed while your project folder is open.

Add OpenCode to Zed like this:

1. Open `Zed`.
2. Open your project or the folder `first-project`.
3. Open the Command Palette with `Cmd + Shift + P`.
4. Search for `zed: acp registry`.
5. Open the ACP Registry.
6. Search for `OpenCode`.
7. Install the OpenCode Agent.
8. Open the Agent Panel through the sparkle icon or through the Command Palette with `agent: new thread`.
9. In the new Thread, choose `OpenCode` as the Agent.

If OpenCode asks you to sign in or connect, follow the instructions.

OpenCode needs access to an AI model. Depending on the workshop setup, this can happen through an OpenCode account, an API key, or another provider.

If you are asked for an API key and do not have one yet, wait for the explanation in the workshop.

You do not need to buy anything before we have clarified together which access we will use.

Note: if you already happen to pay for another Coding Agent, for example `Codex`, `Claude Code`, `Copilot`, or another Agent in Zed, you can also use that. For the shared workshop flow, we use OpenCode.

### 10. Test OpenCode in Terminal

If the Zed connection does not work yet, you can also test OpenCode directly in the Terminal:

1. Open Terminal.
2. Start OpenCode:

```sh
opencode
```

### 11. Create a project folder

A project folder is simply a folder where all files of your project live.

Create a folder on the Desktop:

```sh
cd ~/Desktop
mkdir vibe-coding-projects
cd vibe-coding-projects
mkdir first-project
cd first-project
```

Check where you are:

```sh
pwd
```

You should see a path that ends roughly like this:

```text
Desktop/vibe-coding-projects/first-project
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

Go to your project folder in Terminal:

```sh
cd ~/Desktop/vibe-coding-projects/first-project
```

Start OpenCode:

```sh
opencode
```

If OpenCode starts in Terminal or can be selected as an Agent in Zed, you are ready for the workshop.

If OpenCode does not start, check:

- Does `brew --version` output a version number?
- Does `node --version` output a version number?
- Does `npm --version` output a version number?
- Does `opencode --version` output a version number?
- Are you in the right folder?

## What you have learned

You prepared your Mac so you can work on your own project with a Coding Agent.

You also saw that a project does not start with code, but with a simple working environment: account, Package Manager, Editor, Terminal, project folder, and Agent.
