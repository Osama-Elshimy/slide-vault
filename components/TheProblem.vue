<template>
  <div>
    <h1>The Problem</h1>

    <p>Traditional Git workflow has pain points:</p>

    <div class="grid grid-cols-2 gap-8 mt-4">
      <div v-click="1">
        <h3>😫 Context Switching</h3>
        <pre><code class="language-bash"># Need to test PR but mid-work on feature
git stash -u -m "some message"
git checkout pr-branch
# test...
git checkout feature-branch
git stash pop</code></pre>
      </div>

      <div v-click="2">
        <h3>💾 Disk Waste</h3>
        <pre><code class="language-bash"># Need separate env for testing
git clone ../my-project-test
# Now 2x disk usage!</code></pre>
      </div>

      <div v-click="3">
        <h3>⏸️ Blocking Operations</h3>
        <p>Can't run long tests while coding another feature</p>
      </div>

      <div v-click="4">
        <h3>🔄 Lost Progress</h3>
        <p>Forget to stash? Uncommitted changes block branch switch</p>
      </div>
    </div>
  </div>
</template>
