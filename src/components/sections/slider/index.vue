<script lang="ts" setup>
import SliderCard from '../../shared/slider-card/index.vue'
import dubai from '../../../assets/img/content/location/dubai-creek.png'

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
			<div class="arrow-left"> -- </div>

			<!-- {{ for }} -->
			<SliderCard v-for="{ image, title, info, desc, cost, currency } in sliderCards" :image="image" :title="title"
				:info="info" :desc="desc" :cost="cost" :currency="currency" />

			<div class="arrow-right">--</div>

		</div>
	</div>
</template>

<style lang="scss" scoped>
.slider {
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
}
</style>