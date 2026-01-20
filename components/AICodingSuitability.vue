<template>
  <div>
    <h1>AI Coding Suitability</h1>

    <p>Git worktrees are ideal for AI-assisted development:</p>

    <div class="grid grid-cols-2 gap-6 mt-4">
      <div v-click="1">
        <h3>🤖 Isolated AI Sessions</h3>

        <p>Each AI conversation gets its own worktree</p>
        <ul>
          <li>No cross-contamination of changes</li>
          <li>Easy to compare AI suggestions side-by-side</li>
          <li>Rollback is simple (just remove worktree)</li>
        </ul>
      </div>

      <div v-click="2">
        <h3>🔀 Parallel AI Work</h3>

        <p>Multiple AI agents working simultaneously:</p>
        <pre><code class="language-bash">../project-ai-feature-a    # Claude on feature A
../project-ai-refactor     # Claude on refactor
../project-main            # Your work continues</code></pre>
      </div>

      <div v-click="3">
        <h3>🧪 Safe Experimentation</h3>
        <pre><code class="language-bash"># AI suggests big refactor
git worktree add ../ai-refactor-sandbox -b ai-sandbox
cd ../ai-refactor-sandbox
# Let AI go wild here
# If good: merge to main
# If bad: just delete worktree</code></pre>
      </div>
    </div>
  </div>
</template>
