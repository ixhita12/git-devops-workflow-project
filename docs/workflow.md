# Git Workflow Documentation

## Overview

This document explains the Git workflow followed in this project.

The workflow demonstrates:

- Branch-based development
- Feature implementation
- Pull Request creation
- Code review process
- Merging changes into the main branch
- Version tagging



## Workflow Steps

### 1. Create Development Branch

```bash
git checkout -b dev
```

The development branch is used for implementing features before merging into the main branch.



### 2. Create Feature Branch

Example:

```bash
git checkout -b feature/add-backup-script
```

Feature branches are created for individual tasks or enhancements.


### 3. Make Changes

Files are modified according to project requirements.

Example:

- Added backup script
- Added workflow documentation
- Updated release notes



### 4. Commit Changes

```bash
git add .
git commit -m "feat: add backup script"
```

Meaningful commit messages help track project history.


### 5. Push Branch

```bash
git push origin feature/add-backup-script
```

The feature branch is pushed to GitHub.



### 6. Create Pull Request

A Pull Request (PR) is created to merge changes into the main branch.

Benefits:

- Review changes
- Discuss improvements
- Maintain code quality



### 7. Merge Pull Request

After review, the Pull Request is merged into the main branch.



### 8. Create Release Tag

```bash
git tag -a v1.0.0 -m "First stable release"
git push origin v1.0.0
```

Tags are used to mark project versions.



## Workflow Summary

Feature Branch
↓
Commit Changes
↓
Push Branch
↓
Create Pull Request
↓
Review & Merge
↓
Create Release Tag