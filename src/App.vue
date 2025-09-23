<template>
  <main>
    <div>
      <router-view />
    </div>
  </main>
</template>

<script setup lang="ts"></script>

<style scoped>
main {
  margin: 0;
  padding: 0;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/* 전역 스타일 리셋 */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  margin: 0;
  padding: 0;
}
</style>
