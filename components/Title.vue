<template>
  <div class="h-full flex flex-col justify-between gap-[250px] relative">
    <div>
      <h1>Git Worktrees</h1>
      <p>Work on multiple branches simultaneously</p>
    </div>

    <Info />

    <div v-click class="text-red-500 text-[500px] absolute bottom-0 end-0">
      <img src="../public/force-push.png" class="w-[400px] h-[300px]" />
    </div>
  </div>
</template>
