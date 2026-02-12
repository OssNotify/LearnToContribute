# Setting Up Git

Git is the version control system used by nearly every open source project. Before you can contribute, you need to install Git and configure it with your identity.

## Step 1: Install Git

### macOS

Git comes pre-installed on most Macs. Open your terminal and check:

```bash
git --version
```

If it's not installed, you'll be prompted to install it. Alternatively, install it with [Homebrew](https://brew.sh):

```bash
brew install git
```

### Windows

Download Git from [git-scm.com](https://git-scm.com/download/win) and run the installer. Use the default settings.

After installation, open **Git Bash** (installed with Git) to use Git commands.

### Linux

Use your package manager:

```bash
# Ubuntu / Debian
sudo apt update && sudo apt install git

# Fedora
sudo dnf install git
```

## Step 2: Configure Your Identity

Git needs to know who you are so your contributions are attributed to you. Run these commands with your own name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Use the same email address you use for your GitHub account so your commits are linked to your profile.

## Step 3: Create a GitHub Account

If you don't already have one, create a free account at [github.com](https://github.com).

Your GitHub profile is where your contributions will appear. Choose a username you're happy with — it becomes part of your developer identity.

## Step 4: Set Up Authentication

To push code to GitHub, you need to authenticate. The recommended method is SSH keys.

### Generate an SSH Key

```bash
ssh-keygen -t ed25519 -C "your.email@example.com"
```

Press Enter to accept the default file location, then set a passphrase (or press Enter for none).

### Add Your Key to GitHub

1. Copy your public key:

```bash
# macOS
cat ~/.ssh/id_ed25519.pub | pbcopy

# Linux
cat ~/.ssh/id_ed25519.pub
```

2. Go to [GitHub SSH Settings](https://github.com/settings/keys)
3. Click **New SSH key**
4. Paste your key and save

### Test the Connection

```bash
ssh -T git@github.com
```

You should see: `Hi username! You've successfully authenticated`.

## Verify Your Setup

Run these commands to confirm everything is working:

```bash
git --version
git config user.name
git config user.email
```

You should see your Git version, name, and email.

## What's Next?

Your tools are ready. Next, learn how to [Fork and Clone](03-forking-and-cloning.md) a repository.
