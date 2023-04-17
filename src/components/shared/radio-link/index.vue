<script lang="ts" setup>
defineProps<{ title: string, name: string }>()
</script>

<template>
	<li class="radio-item">
		<label :for="name">
			<input type="radio" name="title" :id="name" />
			{{ title }}
		</label>
	</li>
</template>

<style lang="scss" scoped>
.radio-item {
	display: flex;
	justify-content: left;
	align-items: center;
	gap: 13px;


	:nth-child(1) {
		margin-top: 0;
	}

	label {
		font-family: 'Lato';
		font-style: normal;
		font-weight: 500;
		font-size: 16px;
		line-height: 19px;
		text-transform: uppercase;
		cursor: pointer;
	}
}
</style>