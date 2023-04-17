<script lang="ts" setup>
defineProps<{ image: string, title: string, desc: string }>()
</script>

<template>
	<div class="card">
		<img :src="image" :alt="title" />
		<div class="content">
			<h2 class="title">{{ title }} </h2>
			<p class="desc">
				{{ desc }}
			</p>

		</div>
	</div>
</template>

<style lang="scss" scoped>
.card {
	position: relative;

	.content {
		height: 175px;
		position: absolute;
		bottom: 0;
		background: rgba(255, 255, 255, 0.85);
		backdrop-filter: blur(10px);
		padding: 27px 48px;

		.title {
			font-family: 'Alethia Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 28.4536px;
			line-height: 38px;
			text-transform: uppercase;
			color: #071C35;
		}

		.desc {
			font-family: 'Lato';
			font-style: normal;
			font-weight: 300;
			font-size: 15.1753px;
			line-height: 23px;
			color: #071C35;
		}
	}

}
</style>