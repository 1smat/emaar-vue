<script setup lang="ts">

defineProps<{ image: string, title: string }>()

</script>

<template>
	<div class="modal">
		<img :src="image" alt="" />
		<div class="inner">
			<div class="title">
				{{ title }}
			</div>
		</div>

	</div>
</template>

<style lang="scss" scoped>
.modal {
	position: relative;
	z-index: 4;
	width: 200px;
	height: 200px;
	background: #FFFFFF;
	border: 1px solid rgba(0, 0, 0, 0.05);
	box-shadow: 0px 0px 14px 3px rgba(0, 0, 0, 0.03);

	left: -79px;
	top: -218px;




	img {}

	.inner {
		height: 80px;
		display: flex;
		align-items: center;
		justify-content: center;

		.title {
			font-family: 'Lato';
			font-style: normal;
			font-weight: 500;
			font-size: 16px;
			line-height: 19px;
			text-align: center;
			text-transform: uppercase;

			color: #071C35;
		}
	}
}
</style>