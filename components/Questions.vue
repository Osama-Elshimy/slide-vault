<template>
  <div class="flex justify-center items-center h-full text-center">
    <div>
      <h1>Questions?</h1>

      <div class="text-sm opacity-75 mt-8">
        <p>Try it out:</p>
        <pre><code class="language-bash">git worktree add ../my-first-worktree -b experiment/test</code></pre>
      </div>

      <PoweredBySlidev mt-10 />
    </div>
  </div>
</template>

<script setup lang="ts">
import PoweredBySlidev from '@slidev/client/builtin.vue'
</script>
