<script setup lang="ts">

import emaar from '../../assets/img/emaar.svg';

defineProps<{ msg?: string }>()


</script>

<template>
	<section class="card">
		<img class="title" :src="emaar" alt="" />



		<hr width="100" />

		<p class="desc">
			Dubai creek <br /> harbour
		</p>

		<section class="info">
			<div class="item">
				<h6 class="title">20%</h6>
				<p class="desc">to booka unit</p>
			</div>
			<div class="item">
				<h6 class="title">4 years</h6>
				<p class="desc">payment plan</p>
			</div>
			<div class="item">
				<h6 class="title">aed 2.2mln</h6>
				<p class="desc">prices from</p>
			</div>
		</section>


	</section>
</template>

<style scoped lang="scss">
.card {
	position: absolute;
	width: 382px;
	height: 431px;
	left: 70px;
	bottom: 70px;
	background: rgba(7, 28, 53, 0.5);
	backdrop-filter: blur(7.5px);
	padding-left: 30px;
	padding-top: 30.07px;


	// .title {}

	hr {
		margin-top: 29.67px;
	}

	.desc {
		margin-top: 30px;
		font-family: 'Alethia Pro';
		font-style: normal;
		font-weight: 400;
		font-size: 30px;
		line-height: 40px;
		text-transform: uppercase;
		color: #FFFFFF;
	}

	.info {
		display: flex;
		gap: 30px;

		.item {

			.title {
				font-family: 'Alethia Pro';
				font-style: normal;
				font-weight: 400;
				font-size: 20px;
				line-height: 40px;
				text-transform: uppercase;
				color: #FFFFFF;
			}

			.desc {
				font-family: 'Lato';
				font-style: normal;
				font-weight: 400;
				font-size: 16px;
				line-height: 19px;
				color: #C4C4C4;
			}
		}

	}
}
</style>
