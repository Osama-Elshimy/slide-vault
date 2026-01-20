<template>
  <div class="grid grid-cols-2 gap-16">
    <div>
      <h1>Basic Syntax: Manage</h1>

      <p>Commands to manage your worktrees:</p>

      <pre><code class="language-bash"># List all worktrees
git worktree list

# Show worktree details
git worktree list --porcelain

# Move a worktree
git worktree move ../old-path ../new-path

# Remove a worktree
git worktree remove ../my-project-feature

# Clean up stale worktrees
git worktree prune</code></pre>
    </div>

    <div class="text-sm">
      <h3>Common Operations</h3>

      <v-clicks>
        <section>
          <strong>List output shows:</strong>
          <ul>
            <li>Worktree path</li>
            <li>Branch name/commit</li>
            <li>Status (detached, prunable, etc.)</li>
          </ul>
        </section>

        <section>
          <strong>Remove vs Prune:</strong>
          <ul>
            <li><code>remove</code> - Deletes worktree cleanly</li>
            <li><code>prune</code> - Cleans up stale refs after manual deletion</li>
          </ul>
        </section>

        <section>
          <strong>Lock/Unlock:</strong>
          <pre><code class="language-bash">git worktree lock ../my-project
git worktree unlock ../my-project</code></pre>
        </section>
      </v-clicks>
    </div>
  </div>
</template>
