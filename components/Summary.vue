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

    <div class="mt-8 text-sm opacity-75 text-center">
      <a href="https://git-scm.com/docs/git-worktree">Official Docs</a>
      ·
      <a
        href="https://www.youtube.com/watch?v=aolI_Rz0ZqY&pp=ygUZc28geW91IHRoaW5rIHlvdSBrbm93IGdpdA%3D%3D"
        >So you think you know git?</a
      >
    </div>
  </div>
</template>
