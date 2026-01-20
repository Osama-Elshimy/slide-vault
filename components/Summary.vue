<template>
  <h1 class="text-center">Summary</h1>
  <div class="text-center">
    <div class="grid grid-cols-3 gap-4 text-start">
      <section>
        <h2>✅ Key Takeaways</h2>
        <ul>
          <li>Worktrees enable simultaneous branch work without stashing</li>
          <li>Share <code>.git</code>, separate working directories</li>
          <li>Perfect for hotfixes, code reviews, parallel testing</li>
          <li>Great for AI coding isolation</li>
        </ul>
      </section>

      <section>
        <h2>✅ When to Use</h2>
        <ul>
          <li>Hot fixes needed while coding feature</li>
          <li>Testing multiple branches/PRs</li>
          <li>Long-running tasks blocking development</li>
          <li>AI wants to experiment safely</li>
        </ul>
      </section>

      <section>
        <h2>❌ When NOT to Use</h2>
        <ul>
          <li>Simple branch switching (checkout is fine)</li>
          <li>Very short-lived operations</li>
          <li>Single developer, sequential work</li>
        </ul>
      </section>
    </div>
  </div>
</template>
