# Contributors

Welcome! This is where you make your first open source contribution.

Add your profile by creating a JSON file in this directory. It's a real pull request to a real repository — and a great way to practice the workflow.

## How to Add Your Profile

### 1. Fork and Clone

If you haven't already, [fork this repository](https://github.com/ossnotify/LearnToContribute/fork) and clone it to your computer:

```bash
git clone https://github.com/YOUR-USERNAME/LearnToContribute.git
cd LearnToContribute
```

### 2. Create a Branch

```bash
git checkout -b add-profile-YOUR-USERNAME
```

### 3. Copy the Template

```bash
cp contributors/example.json contributors/YOUR-USERNAME.json
```

### 4. Edit Your Profile

Open `contributors/YOUR-USERNAME.json` and fill it in:

```json
{
  "name": "Your Name",
  "github": "your-github-username",
  "skills": ["JavaScript", "Python", "React"],
  "message": "Hello from my first open source contribution!"
}
```

**Guidelines:**
- Use your actual GitHub username as the filename
- List 1-5 skills or technologies you know or are learning
- Keep your message friendly and appropriate
- Don't modify other contributors' files

### 5. Commit and Push

```bash
git add contributors/YOUR-USERNAME.json
git commit -m "Add contributor profile for YOUR-USERNAME"
git push origin add-profile-YOUR-USERNAME
```

### 6. Open a Pull Request

Go to the original repository on GitHub and click **Compare & pull request**. Fill out the template and submit.

That's it! A maintainer will review and merge your profile.

## Need Help?

- Read the full guide: [Making Your First Pull Request](../guides/04-making-your-first-pr.md)
- [Open an issue](../../issues) if you're stuck

## Contributors

Thanks to everyone who has contributed!

<!-- Contributors will appear here as profiles are added -->
