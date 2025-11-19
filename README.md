# Task 4: Git Branching and Workflow

This repository is a practical demonstration of common Git workflows for feature development, teamwork, and merging strategies. The task guides you through the creation and management of branches for proper version control and collaboration.

## Task Objectives

- Create and switch between multiple branches.
- Make and merge changes across branches.
- Simulate individual contributions in a team workflow.
- Resolve potential merge conflicts.

## Steps and Commands

### 1. Repository Setup

```sh
# Clone the remote repository
git clone <repo-url>
cd <repo-name>
```

### 2. Branch Creation

```sh
# Create a feature branch and switch to it
git checkout -b feature

# Create a dev branch and switch to it
git checkout -b dev
```

### 3. Making Changes

- Edit/add files on `dev` and `feature` branches.
<p> This commit is from the dev branch </p>

<p> This commit is from the feature branch</p>

```sh
# Stage and commit changes
git add .
git commit -m "your commit message"
```

### 4. Pushing Branches

```sh
# Push your branches to the remote repository
git push origin dev
git push origin feature
```

### 5. Merging Workflow

- Merge changes from `feature` branch into `dev` branch.

```sh
git checkout dev
git merge feature
```

- If there are merge conflicts, resolve them in the files, then:

```sh
git add .
git commit -m "Resolve merge conflicts"
```

### 6. Final Merge to Main

- After development is complete, merge `dev` into `main`:

```sh
git checkout main
git merge dev
```
