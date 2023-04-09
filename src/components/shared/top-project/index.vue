<script setup lang="ts">

defineProps<{ image: string, title: string, info: string }>()

</script>

<template>
	<div class="item">
		<img :src="image" alt="" />
		<div class="inner">
			<div class="data">
				<div class="title">
					{{ title }}
				</div>
				<div class="info">
					{{ info }}
				</div>
			</div>
		</div>

	</div>
</template>

<style lang="scss" scoped>
.item {
	display: flex;
	flex-direction: column;
	border: 1px solid rgba(7, 28, 53, 0.1);
	padding: 15px;
	position: relative;

	.inner {
		position: relative;

		.data {

			padding-top: 22px;
			padding-bottom: 22px;
			padding-left: 15px;
			background: rgba(255, 255, 255, 0.85);
			backdrop-filter: blur(7.5px);

			width: 100%;
			position: absolute;
			bottom: 0;

			.title {
				font-family: 'Alethia Pro';
				font-style: normal;
				font-weight: 400;
				font-size: 25px;
				line-height: 25px;
				/* identical to box height */
				text-transform: uppercase;

				color: #071C35;
			}

			.info {
				font-family: 'Lato';
				font-style: normal;
				font-weight: 400;
				font-size: 16px;
				line-height: 19px;
				text-transform: uppercase;

				color: #071C35;
				margin-top: 7px;

			}
		}
	}






}
</style>