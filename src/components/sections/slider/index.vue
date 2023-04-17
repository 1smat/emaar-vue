<script lang="ts" setup>
import SliderCard from '../../shared/slider-card/index.vue'
import dubai from '../../../assets/img/content/location/dubai-creek.png'
import arrowRightIcon from '../../../assets/img/icons/right-arrow.svg'
import arrowLeftIcon from '../../../assets/img/icons/left-arrow.svg'

const sliderCards = [
	{
		image: dubai,
		title: "title",
		info: "bedrooms 1-3",
		desc: "Creek Rise comprises two beautifully designed residential high-rises with unparalleled views overlooking the Creek Island’s lush parkland, set in a family-oriented neighbourhood.",
		cost: "2 228 888",
		currency: "aed"
	}

]

</script>


<template>
	<div class="slider">
		<div class="header">
			<h2 class="units">AVAILABLE UNITS</h2>
			<div class="count">
				<span class="current"> 1</span> /
				<span class="all"> 3</span>
			</div>
		</div>
		<div class="content">
			<SliderCard v-for="{ image, title, info, desc, cost, currency } in sliderCards" :image="image" :title="title"
				:info="info" :desc="desc" :cost="cost" :currency="currency" />
		</div>
		<div>
			<div class="arrow-left">
				<img :src="arrowLeftIcon" alt="Arrow Left">
			</div>

			<div class="arrow-right">
				<img :src="arrowRightIcon" alt="Arrow Right" />
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.slider {
	padding: 40px;
	position: relative;

	.header {
		display: flex;
		justify-content: space-between;
		padding: 0 110px;

		.units {
			font-family: 'Alethia Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 30px;
			line-height: 40px;
			text-transform: uppercase;
			color: #071C35;
		}

		.count {
			font-family: 'Lato';
			font-style: normal;
			font-weight: 300;
			font-size: 30px;
			line-height: 40px;
			text-transform: uppercase;

			.current {
				color: #071C35;
			}

			.all {
				color: #777777;
			}
		}
	}

	.content {
		display: flex;
		justify-content: center;
	}

	.arrow-right {
		img {
			position: absolute;
			top: 280px;
			right: 0;
		}
	}

	.arrow-left {
		img {
			position: absolute;
			top: 280px;
			left: 0;
		}
	}
}
</style>