<script lang="ts" setup>
import badIcon from '../../../assets/img/icons/bad.svg'
defineProps<{ image: string, title: string, info: string, desc: string, cost: string, currency: string }>()
</script>

<template>
	<div class="slider-card">
		<img :src="image" :alt="title" />
		<div class="card-content">
			<h2 class="title">{{ title }} </h2>
			<h6 class="info"> <img :src="badIcon" alt="bad icon" /> {{ info }} </h6>
			<p class="desc">{{ desc }} </p>
			<h5 class="cost"> from
				<span class="currency"> {{ currency }} </span>
				<span class="value"> {{ " " + cost }} </span>
			</h5>
			<button class="button"> get details </button>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.slider-card {
	display: flex;
	width: 750px; // 220


	img {
		width: 440px;
	}

	.card-content {
		padding: 30px;
		width: 310px;
		display: flex;
		flex-direction: column;
		gap: 15px;
		background: rgba(255, 255, 255, 0.85);
		filter: drop-shadow(0px 20px 30px rgba(0, 0, 0, 0.07));

		// box-shadow: red 2px 4px;

		.title {
			font-family: 'Alethia Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 30px;
			line-height: 40px;
			text-transform: uppercase;
			color: #071C35;
		}

		.info {
			display: flex;
			justify-content: flex-start;
			align-items: center;
			gap: 10px;

			img {
				width: 20px;
			}
		}

		.desc {
			font-family: 'Lato';
			font-style: normal;
			font-weight: 300;
			font-size: 16px;
			line-height: 24px;
			color: #777777;

		}

		.cost {
			font-family: 'Lato';
			font-style: normal;
			font-weight: 400;
			font-size: 16px;
			line-height: 40px;
			text-transform: uppercase;
			color: #071C35;
		}

		.button {
			font-family: 'Lato';
			font-style: normal;
			font-weight: 400;
			font-size: 14px;
			line-height: 17px;
			text-align: center;
			text-transform: uppercase;
			color: #FFFFFF;
			background: #071C35;
			padding: 12px 82px;
		}
	}
}
</style>