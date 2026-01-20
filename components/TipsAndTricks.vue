<template>
  <div>
    <h1>Tips & Tricks</h1>

    <div class="grid grid-cols-2 gap-20 mt-4">
      <div v-click="1">
        <h3>🚀 Hot Fixes</h3>
        <pre><code class="language-bash"># Critical bug comes in, you're mid-feature
git worktree add ../hotfix -b hotfix/crash
cd ../hotfix
# fix, test, commit, push
cd ../my-project
# Continue feature work uninterrupted</code></pre>
      </div>

      <div v-click="2">
        <h3>📝 Code Reviews</h3>
        <pre><code class="language-bash"># Review and test PRs locally
git worktree add ../review-pr-123 origin/pr-123</code></pre>
      </div>

      <div v-click="3">
        <h3>🏷️ Naming Convention</h3>
        <p>Use descriptive paths:</p>
        <pre><code class="language-bash">../project-feature-auth
../project-hotfix-login
../project-test-api</code></pre>
      </div>

      <div v-click="4">
        <h3>🧪 Parallel Testing</h3>
        <pre><code class="language-bash"># Run tests in background worktree
cd ../my-project-test
npm test &
cd ../my-project
# Continue coding...</code></pre>
      </div>

      <div v-click="5">
        <h3>🔄 CI/CD Workflows</h3>
        <pre><code class="language-bash"># CI creates worktree for testing
git worktree add ../build-temp HEAD~1
cd ../build-temp && npm run build</code></pre>
      </div>

      <div v-click="6">
        <h3>🧹 Cleanup</h3>
        <pre><code class="language-bash"># Clean all finished worktrees
git worktree prune
git worktree list  # Check what remains</code></pre>
      </div>
    </div>
  </div>
</template>
