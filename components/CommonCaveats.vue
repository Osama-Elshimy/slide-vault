<template>
  <div>
    <h1>Common Caveats</h1>

    <div class="grid grid-cols-2 gap-40 mt-4">
      <div v-click="1">
        <h3>⚠️ Same Branch Limit</h3>

        <p>
          Can't checkout the <strong>same branch</strong> in multiple worktrees
        </p>

        <pre><code class="language-bash"># This will fail if main is already checked out
git worktree add ../wt2 main
# fatal: '../wt2' is already checked out at '.'</code></pre>

        <h3 class="mt-4">⚠️ Manual Deletion</h3>

        <p>Don't <code>rm -rf</code> worktree directories manually</p>
        <p v-click="2">→ Use <code>git worktree remove</code> instead</p>
        <p v-click="3">
          → Or run <code>git worktree prune</code> after deletion
        </p>
      </div>

      <div v-click="4">
        <h3>⚠️ Independent Operations</h3>

        <p>Each worktree operates independently:</p>
        <ul>
          <li>Rebase/merge conflicts resolved per worktree</li>
          <li>Hooks run in each worktree separately</li>
        </ul>

        <h3 class="mt-4 text-nowrap">
          ⚠️ <code>git fetch</code> Different Behavior
        </h3>
        <ul>
          <li>
            <code>git fetch</code> in a bare repo doesn't update
            <code>refs/remotes/origin</code>
          </li>
          <span>
            → Manually map the refspec so fetch behaves like a standard clone
            <code v-mark.red class="block"
              >git config remote.origin.fetch
              "+refs/heads/*:refs/remotes/origin/*"</code
            >
          </span>
        </ul>
      </div>
    </div>
  </div>
</template>
