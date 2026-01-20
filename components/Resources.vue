<template>
  <div class="flex h-full text-center">
    <div>
      <h1>Resources</h1>

      <div class="grid grid-cols-2 gap-8 mt-12 text-start">
        <section>
          <h2>📚 Documentation</h2>
          <ul>
            <li>
              <a href="https://git-scm.com/docs/git-worktree" target="_blank">
                Official Git Worktree Docs
              </a>
            </li>
            <li>
              <a href="https://git-scm.com/docs" target="_blank">
                Git Reference Manual
              </a>
            </li>
          </ul>
        </section>

        <section>
          <h2>🎥 Videos</h2>
          <ul>
            <li>
              <a
                href="https://www.youtube.com/watch?v=aolI_Rz0ZqY"
                target="_blank"
              >
                "So You Think You Know Git"
              </a>
            </li>
          </ul>
        </section>

        <section class="col-span-2">
          <h2>📦 Slides</h2>
          <ul>
            <li>
              <a
                href="https://github.com/Osama-Elshimy/slide-vault/tree/git-worktrees"
                target="_blank"
              >
                This presentation on GitHub
              </a>
            </li>
          </ul>
        </section>

        <section>
          <h2>🧪 Try It</h2>
          <pre><code class="language-bash max-w-full text-wrap">git clone https://github.com/Osama-Elshimy/slide-vault <span v-mark.circle.red>--bare</span></code></pre>
        </section>
      </div>
    </div>
  </div>

  <PoweredBySlidev class="text-center mx-auto" />
</template>
