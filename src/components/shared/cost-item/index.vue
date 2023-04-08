<script setup lang="ts">

defineProps<{ cost: number, phrase: string }>()

</script>

<template>
	<div class="item">
		<div class="cost">
			$ {{ cost }} bln
		</div>
		<div class="phrase">
			{{ phrase }}
		</div>
	</div>
</template>

<style lang="scss" scoped>
.item {
	display: flex;
	flex-direction: column;

	.cost {
		font-family: 'Alethia Pro';
		font-style: normal;
		font-weight: 400;
		font-size: 44px;
		line-height: 44px;
		/* identical to box height */

		color: #071C35;
	}

	.phrase {
		text-align: left;
		font-family: 'Lato';
		font-style: normal;
		font-weight: 300;
		font-size: 16px;
		line-height: 19px;

		text-transform: uppercase;

		color: #777777;
	}
}
</style>