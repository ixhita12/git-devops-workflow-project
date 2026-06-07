# Git Branching Strategy

## Overview

This project follows a feature-based branching strategy commonly used in DevOps and software development teams.

The goal is to keep the main branch stable while allowing new features and updates to be developed independently.



## Branch Structure

### Main Branch

```text
main
```

The production-ready branch.

Responsibilities:

- Stable codebase
- Approved changes only
- Release versions



### Development Branch

```text
dev
```

The integration branch where feature branches are combined before final release.

Responsibilities:

- Feature testing
- Integration validation
- Pre-release verification



### Feature Branches

Examples:

```text
feature/add-backup-script
feature/git-documentation
feature/release-notes-update
```

Responsibilities:

- Develop individual features
- Isolate changes
- Prevent impact on the main branch



## Workflow

```text
main
 │
 └── dev
      │
      ├── feature/add-backup-script
      │        ↓
      │      Pull Request
      │        ↓
      │      Merge
      │
      ├── feature/git-documentation
      │        ↓
      │      Pull Request
      │        ↓
      │      Merge
      │
      └── feature/release-notes-update
               ↓
             Pull Request
               ↓
             Merge
```



## Benefits

- Better collaboration
- Easy code review process
- Reduced merge conflicts
- Stable production branch
- Improved release management
- Clear project history



## Best Practices Used

- Meaningful branch names
- Small and focused commits
- Pull Request based workflow
- Version tagging
- Documentation for every change


## Version

Current Release:

```text
v1.0.0
```

This version represents the first stable release of the project.