# Making Your First Pull Request

A pull request (PR) is how you propose changes to an open source project. You make changes in your fork, then ask the project maintainers to review and merge them.

Let's walk through the entire process using this repository.

## Step 1: Create a Branch

Always create a new branch for your changes. Never work directly on `main`.

```bash
git checkout -b add-my-profile
```

This creates a new branch called `add-my-profile` and switches to it.

### Why Branch?

- Keeps your `main` branch clean and in sync with upstream
- Each PR gets its own branch, so you can work on multiple contributions at once
- Makes it easy to start over if something goes wrong

## Step 2: Make Your Changes

For your first PR, add your contributor profile. Create a new file in the `contributors/` directory:

```bash
cp contributors/example.json contributors/your-github-username.json
```

Open the file and fill in your details:

```json
{
  "name": "Your Name",
  "github": "your-github-username",
  "skills": ["JavaScript", "Python"],
  "message": "Excited to start contributing!"
}
```

## Step 3: Stage Your Changes

Tell Git which files you want to include in your commit:

```bash
git add contributors/your-github-username.json
```

Check what's staged:

```bash
git status
```

You should see your new file listed under "Changes to be committed."

## Step 4: Commit Your Changes

Save your changes with a descriptive message:

```bash
git commit -m "Add contributor profile for your-github-username"
```

A good commit message:
- Starts with a verb (Add, Fix, Update, Remove)
- Is short but descriptive
- Explains what changed, not how

## Step 5: Push to Your Fork

Upload your branch to GitHub:

```bash
git push origin add-my-profile
```

## Step 6: Open the Pull Request

1. Go to your fork on GitHub (`https://github.com/YOUR-USERNAME/LearnToContribute`)
2. You'll see a banner saying your branch was recently pushed — click **Compare & pull request**
3. Fill out the PR template:
   - Write a clear title (e.g., "Add contributor profile for your-github-username")
   - Describe what you changed in the body
   - Check the relevant boxes in the checklist
4. Click **Create pull request**

## What Happens Next?

After you submit your PR:

1. **Automated checks** may run (like the welcome bot greeting you)
2. A **maintainer reviews** your changes
3. They may **request changes** — don't worry, this is normal and part of the process
4. Once approved, your PR gets **merged** into the main project

## Responding to Feedback

If a maintainer requests changes:

1. Make the changes on the same branch locally
2. Commit and push again:

```bash
git add .
git commit -m "Address review feedback"
git push origin add-my-profile
```

Your PR will automatically update with the new changes.

## After Your PR is Merged

Clean up your local branches:

```bash
git checkout main
git pull upstream main
git branch -d add-my-profile
```

Congratulations — you've just made your first open source contribution!

## What's Next?

Learn about [Understanding Issues](05-understanding-issues.md) to find more ways to contribute.
