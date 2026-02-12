# Forking and Cloning

Before you can make changes to an open source project, you need your own copy of the code. This involves two steps: **forking** (creating your copy on GitHub) and **cloning** (downloading it to your computer).

## What is a Fork?

A fork is your personal copy of someone else's repository on GitHub. It lives under your GitHub account and is completely independent — you can make any changes you want without affecting the original project.

When you're ready, you submit a **pull request** to propose merging your changes back into the original.

## Step 1: Fork the Repository

Let's practice with this repository:

1. Go to the [LearnToContribute repository](https://github.com/ossnotify/LearnToContribute) on GitHub
2. Click the **Fork** button in the top-right corner
3. Select your GitHub account as the destination

GitHub will create a copy at `https://github.com/YOUR-USERNAME/LearnToContribute`.

## Step 2: Clone Your Fork

Now download your fork to your computer:

```bash
git clone https://github.com/YOUR-USERNAME/LearnToContribute.git
```

Replace `YOUR-USERNAME` with your actual GitHub username.

This creates a `LearnToContribute` folder on your computer with all the project files.

```bash
cd LearnToContribute
```

## Step 3: Add the Upstream Remote

To keep your fork up to date with the original project, add it as a remote called `upstream`:

```bash
git remote add upstream https://github.com/ossnotify/LearnToContribute.git
```

Verify your remotes:

```bash
git remote -v
```

You should see:
```
origin    https://github.com/YOUR-USERNAME/LearnToContribute.git (fetch)
origin    https://github.com/YOUR-USERNAME/LearnToContribute.git (push)
upstream  https://github.com/ossnotify/LearnToContribute.git (fetch)
upstream  https://github.com/ossnotify/LearnToContribute.git (push)
```

- **origin** — Your fork (where you push changes)
- **upstream** — The original project (where you pull updates from)

## Keeping Your Fork Up to Date

Before starting new work, pull the latest changes from upstream:

```bash
git fetch upstream
git merge upstream/main
```

This ensures your fork has the latest code from the original project.

## Key Concepts

| Term | What It Means |
|------|---------------|
| **Fork** | Your copy of a repo on GitHub |
| **Clone** | Downloading a repo to your computer |
| **Origin** | Your fork (remote) |
| **Upstream** | The original project (remote) |
| **Remote** | A version of the repo hosted on GitHub |

## What's Next?

You have a local copy of the project. Now let's [Make Your First Pull Request](04-making-your-first-pr.md).
