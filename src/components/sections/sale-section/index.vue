<script setup lang="ts">
import CostItem from '../../shared/cost-item/index.vue'

import background from '../../../assets/img/sale-image.png'
import logo from '../../../assets/img/logo.png'


</script>

<template>
	<section class="sale">
		<div class="images">
			<div class="background">
				<img :src="logo" alt="" />
			</div>
			<div class="logo">
				<img :src="background" alt="" />
			</div>
		</div>
		<div class="info">
			<h2 class="title">AVAILABLE HOMES FOR SALE BY EMAAR PROPERTIES</h2>
			<div class="desc">
				Emaar Properties is one of the world’s most valuable and admired real estate development
				companies. With proven competencies in properties, shopping malls & retail and hospitality & leisure.Emaar
				Properties is one of the world’s most valuable and admired real estate development companies
			</div>
			<div class="prices">

				<CostItem :cost="10.9" :phrase="`Market cap`" />
				<CostItem :cost="7.7" :phrase="`Revenue`" />
				<CostItem :cost="1" :phrase="`Net profit`" />

			</div>
			<br />
			<br>
			<div class="button">
				<a href="">SEE MORE</a>
			</div>
		</div>
	</section>
</template>

<style lang="scss" scoped>
.sale {
	display: flex;
	// justify-content: space-between;
	gap: 54px;
	padding-top: 136px;


	.images {
		width: 498px;
		height: 547px;

		.background {
			position: relative;

			img {
				position: absolute;

			}
		}
	}

	.info {
		display: flex;
		flex-direction: column;
		max-width: 657px;
		padding-top: 75px;

		.title {
			font-family: 'Alethia Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 44px;
			line-height: 120%;
			/* or 53px */
			text-transform: uppercase;

			color: #071C35;

		}

		.desc {
			font-family: 'Lato';
			font-style: normal;
			font-weight: 300;
			font-size: 16px;
			line-height: 24px;
			/* or 150% */

			color: #777777;

			padding-top: 30px;
		}

		.prices {
			padding-top: 50px;
			display: flex;
			justify-content: space-between;
			flex-basis: 3;
		}

		.button {
			a {
				display: flex;
				align-items: center;
				justify-content: center;
				width: 200px;
				height: 40px;
				font-family: 'Lato';
				font-style: normal;
				font-weight: 400;
				font-size: 16px;
				line-height: 19px;
				text-transform: uppercase;
				color: #FFFFFF;
				background: #071C35;
			}

		}
	}


}
</style>w