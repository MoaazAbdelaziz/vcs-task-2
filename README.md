# Version Control

## Removing Git Branches

This section explains how to delete branches both locally and remotely.

### Delete a Local Branch

To delete a local branch:

```bash
git branch -d branch-name
```

### Delete a Remote Branch

To delete a remote branch from the repository:

```bash
git push origin --delete branch-name
```

## Tags in git

This section explains the difference between annotated tags vs lightweight tags and how to list and delete tags.

### Annotated Tags

- Stored as full objects in Git.
- Contain metadata: tagger's name, email, date, and a tagging message.
- Recommended for releases or public versioning.

### Lightweight Tags

- A simple pointer to a specific commit.
- No metadata or message.
- More like a bookmark — useful for temporary or local tagging.

### Listing tags

To list tags use

```bash
 git tag
```

### Deleting tags locally and remotely

You can delete tags localy and remotely

#### Delete a Local Tag

To delete a local tag:

```bash
git tag -d v1.0
```

#### Delete a Remote Tag

To delete a remote tag from the repository:

```bash
git push origin --delete v(tag_version)
```

## Rebase in git

This section explains when to use rebase.

Rebase is powerful Git command used to streamline a series of commits, keeping a cleaner and more linear project history.

### When to use rebase?

- When you want to write your code without worrying about breaking it up into isolated commits.

- You want to fixup commits before merging.

## Image

![Git Workflow Diagram](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*JLYlSLSK8-AZo8gt9UdYqA.jpeg)
