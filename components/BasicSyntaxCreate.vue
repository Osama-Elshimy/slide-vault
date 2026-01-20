<template>
  <div class="grid grid-cols-2 gap-16">
    <div>
      <h1>Basic Syntax: Create</h1>

      <p>Create new worktrees from your repository:</p>

      <pre><code class="language-bash"><span v-mark.underline.red># git worktree add [path] [branch]</span>
# Create worktree from existing branch
<v-click>git worktree add ./my-project-feature feature-branch</v-click>

# Create worktree with new branch
<v-click>git worktree add ./my-project-experiment -b experiment-branch</v-click>

# Create worktree at specific commit
<v-click>git worktree add ./my-project-old HEAD~5</v-click>

# Create with detached HEAD (remote branch)
<v-click>git worktree add ./my-project-temp origin/pr-123</v-click></code></pre>
    </div>

    <div class="text-sm">
      <div class="absolute top-10 end-10">
        <v-clicks>
          <h3>Parameters</h3>
          <ul>
            <li><code>&lt;path&gt;</code> - Where to create the worktree</li>
            <li><code>&lt;branch&gt;</code> - Existing branch to checkout</li>
            <li><code>-b &lt;new-branch&gt;</code> - Create new branch</li>
            <li><code>--detach</code> - Detached HEAD mode</li>
            <li><code>--checkout</code> - Default behavior</li>
            <li><code>--force</code> - Force checkout (reset)</li>
          </ul>
        </v-clicks>
      </div>

      <pre
        v-mark.red
        class="absolute bottom-10 end-5"
      ><code class="language-bash {all|2|4|6}"># Example directory structure
my-project/              # original repo
├── .git/
├── my-project-feature/  # worktree 1
├── my-project-fix/      # worktree 2
└── my-project-test/     # worktree 3</code></pre>
    </div>
  </div>
</template>
