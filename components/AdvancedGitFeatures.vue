<template>
  <div class="h-full grid grid-cols-2 justify-center gap-4 relative">
    <img
      src="../public/understand-git.png"
      class="w-[250px] absolute -top-5 end-0"
    />

    <v-clicks>
      <div>
        <h1>Advanced Git Features</h1>
        <p class="opacity-75">Powerful tools most developers don't use</p>
      </div>

      <div class="feature col-span-2">
        <strong>git worktrees</strong> — Work on multiple branches
        simultaneously
      </div>

      <div class="feature">
        <strong>git bisect</strong> — Binary search to find bugs
      </div>

      <div class="feature">
        <strong>git rerere</strong> — Reuse recorded conflict resolutions
      </div>

      <div class="feature">
        <strong>git sparse-checkout</strong> — Clone only parts of a repo
      </div>

      <div class="feature">
        <strong>git submodules</strong> — Embed repos within repos
      </div>

      <div class="feature">
        <strong>interactive rebase</strong> — Rewrite history cleanly
      </div>

      <div class="feature">
        <strong>git reflog</strong> — Recover lost commits
      </div>

      <div class="feature col-span-2">
        <strong>git hooks</strong> — Automate workflows
      </div>
    </v-clicks>
  </div>
</template>

<style scoped>
.feature {
  @apply py-2 px-4 border-l-4 border-blue-500 bg-blue-50 bg-opacity-10 rounded-r;
}
</style>
