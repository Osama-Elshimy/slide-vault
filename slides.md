---
theme: seriph
# background: https://source.unsplash.com/collections/94734566/slidev
title: Git Worktrees
info: |
  ## Git Worktrees
  Work on multiple branches simultaneously
drawings:
  persist: false
mdc: true
---

<Title />

---

<AdvancedGitFeatures />

---

<WhatAreGitWorktrees />

```mermaid {scale: 0.9}
graph TD
    Git[.git directory] --> WT1[worktree-main<br/>main branch]
    Git --> WT2[worktree-feature<br/>feature/login]
    Git --> WT3[worktree-fix<br/>hotfix/critical]
    Git --> WT4[worktree-exp<br/>experiment/new-ui]

    style Git fill:#2B90B6,color:#fff
    style WT1 fill:#4EC5B4
    style WT2 fill:#4EC5B4
    style WT3 fill:#4EC5B4
    style WT4 fill:#4EC5B4
```

---

<TheProblem />

---

<WhatWorktreesSolve />

---

<BasicSyntaxCreate />

---

<BasicSyntaxManage />

---

<CommonCaveats />

---

# Tips & Tricks

<div grid="~ cols-2 gap-4" m="t-4">

<div>

### 🚀 Hot Fixes

```bash
# Critical bug comes in, you're mid-feature
git worktree add ./hotfix -b hotfix/crash
cd ./hotfix
# fix, test, commit, push
cd ./my-project
# Continue feature work uninterrupted
```

### 📝 Code Reviews

```bash
# Review and test PRs locally
git worktree add ./review-pr-123 origin/pr-123
```

### 🏷️ Naming Convention

Use descriptive paths:

```bash
./project-feature-auth
./project-hotfix-login
./project-test-api
```

</div>

<div>

### 🧪 Parallel Testing

```bash
# Run tests in background worktree
cd ./my-project-test
npm test &
cd ./my-project
# Continue coding...
```

### 🔄 CI/CD Workflows

```bash
# CI creates worktree for testing
git worktree add ./build-temp HEAD~1
cd ./build-temp && npm run build
```

### 🧹 Cleanup

```bash
# Clean all finished worktrees
git worktree prune
git worktree list  # Check what remains
```

### An alias for the rescue

```bash
git config --global alias.fix-bare 'config remote.origin.fetch "+refs/heads/*:refs/remotes/origin/*"'
```

</div>

</div>

---

<AICodingSuitability />

---

<RealWorldExample />

---

<Summary />

---

<Questions />

---

<Resources />
