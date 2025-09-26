<template>
	<main>
		<div>
			<router-view />
		</div>
	</main>
</template>

<script setup lang="ts">
import { onMounted } from 'vue';

// 환경 변수에서 title 가져와서 설정
onMounted(() => {
	document.title = import.meta.env.VITE_APP_TITLE;
});
</script>

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
