<script setup lang="ts">
import dot from '../../../assets/img/dot.svg'
import creek from '../../../assets/img/content/location/dubai-creek.png'
import LocationModal from '../../shared/location-modal/index.vue';

</script>

<template>
	<section class="location">
		<div class="title-wrapper">
			<h2 class="title">choose the best location for you</h2>
		</div>
		<div class="marks">

			<div class="top">
				<img :src="dot" alt="" v-on:touchmove="1234" />
				<LocationModal :image="creek" :title="`DUBAI CREEK HARBOUR`" />
			</div>
			<div class="mid">
				<img :src="dot" alt="" />
				<LocationModal :image="creek" :title="`DUBAI CREEK HARBOUR`" />

			</div>
			<div class="bot">
				<img :src="dot" alt="" />
				<LocationModal :image="creek" :title="`DUBAI CREEK HARBOUR`" />
			</div>

		</div>
	</section>
</template>

<style lang="scss" scoped>
.location {
	height: 810px;
	background-image: url('../../../assets/img/content/location/map.jpg');
	margin-top: 109px;
	display: flex;
	flex-direction: row;
	position: relative;

	.title-wrapper {
		position: relative;
		width: 457px;


		.title {
			font-family: 'Alethia Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 44px;
			line-height: 120%;
			/* or 53px */
			text-transform: uppercase;

			color: #071C35;

			position: absolute;
			top: 268px;
		}
	}

	.marks {
		width: 843px;
		height: 658px;
		// padding-top: 231px;

		position: relative;

		.modal {
			visibility: hidden;

		}

		img:hover~.modal {
			visibility: visible;
		}

		img {
			cursor: pointer;
			position: relative;
			z-index: 5;
		}



		.top {
			position: relative;
			top: 202px;
			left: 255px;


		}

		.mid {
			position: relative;
			top: 90px;
			left: 150px;
		}

		.bot {
			position: absolute;
			left: -10px;
			bottom: -245px;
		}
	}
}
</style>