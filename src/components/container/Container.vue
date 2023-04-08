<script setup lang="ts">


defineProps<{ children?: any }>()

</script>

<template>
	<div class="container">
		<slot></slot>
	</div>
</template>

<style scoped>
.container {
	width: 1200px;
	margin: 0 auto;
}
</style>
