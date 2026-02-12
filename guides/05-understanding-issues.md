# Understanding Issues

Issues are how open source projects track bugs, feature requests, and tasks. Learning to read and work with issues is essential for finding meaningful contributions.

## What Are Issues?

GitHub issues are like a project's to-do list. They can represent:

- **Bugs** — Something isn't working correctly
- **Feature requests** — Ideas for new functionality
- **Improvements** — Ways to make existing features better
- **Questions** — Requests for help or clarification
- **Tasks** — Work that needs to be done

## Reading an Issue

A well-written issue typically includes:

- **Title** — A short description of the problem or request
- **Description** — Details about what's expected vs. what's happening
- **Labels** — Tags that categorize the issue (bug, enhancement, good first issue, etc.)
- **Assignees** — Who's working on it
- **Comments** — Discussion and updates from contributors

## Finding Issues to Work On

### Labels to Look For

Most beginner-friendly projects use labels to flag easy issues:

| Label | What It Means |
|-------|---------------|
| `good first issue` | Suitable for first-time contributors |
| `help wanted` | Maintainers are looking for help |
| `beginner` / `easy` | Low complexity |
| `documentation` | Writing or fixing docs (no code needed) |
| `bug` | Something is broken |
| `enhancement` | An improvement to existing functionality |

### Before You Start

1. **Read the entire issue** — including all comments
2. **Check if someone is already working on it** — look for linked PRs or comments saying "I'll take this"
3. **Ask to be assigned** — Comment on the issue to let maintainers know you'd like to work on it
4. **Understand the scope** — Make sure you know what a complete solution looks like

## Working on an Issue

### Claiming an Issue

Leave a comment like:

> "Hi! I'd like to work on this issue. Could you assign it to me?"

Most maintainers will respond within a few days. If you don't hear back after a week, it's usually fine to start working on it anyway.

### Linking Your PR to an Issue

When you open your pull request, reference the issue number in the description:

```
Fixes #42
```

or

```
Closes #42
```

This tells GitHub to automatically close the issue when your PR is merged.

### Common keywords that link PRs to issues:

- `Fixes #123` — Closes the issue when merged
- `Closes #123` — Same as Fixes
- `Resolves #123` — Same as Fixes
- `Related to #123` — Links without closing

## Creating Issues

You can also contribute by reporting bugs or suggesting features:

1. Check if a similar issue already exists
2. Use the project's issue template if available
3. Be specific — include steps to reproduce, expected vs. actual behavior, and screenshots if relevant
4. Be respectful — maintainers are often volunteers

## What's Next?

Now that you know how to find and work on issues, learn how to [Find Issues with OSS Notify](06-using-oss-notify.md) to automate the process.
