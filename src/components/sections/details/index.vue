<script setup lang="ts">
import RadioLink from '../../shared/radio-link/index.vue'
import DetailsCard from '../../shared/details-card/index.vue'
import SliderSection from '../slider/index.vue'

import dubaiCreekImg from '../../../assets/img/content/details/dubai-creek.png'
import cove from '../../../assets/img/content/details/cove.png'
import park from '../../../assets/img/content/details/park.png'
import gate from '../../../assets/img/content/details/gate.png'
import urbana from '../../../assets/img/content/details/urbana.png'

</script>

<template>
	<section class="details">
		<div class="navigation">
			<div class="lists">
				<h2 class="title">community</h2>
				<ul class="wrapper">
					<RadioLink :title="`dubai creek harbour`" name="creek" />
					<RadioLink :title="`dubai hills estate`" name="hills" />
					<RadioLink :title="`emaar south`" name="emaar" />
				</ul>
			</div>
			<div class="projects">
				<h2 class="title">Projects</h2>
				<a href="#rise" class="item active">CREEK RISE </a>
				<a href="#cove" class="item">THE COVE </a>
				<a href="#gate" class="item">CREEK GATE </a>
			</div>

		</div>

		<div class="projects-content" id="rise">
			<div class="content">
				<DetailsCard :image="dubaiCreekImg" title="creek rise"
					desc="At Dubai Creek Harbour, you will experience more of what really matters. More laughs shared with friends More memories made. A thriving community to live, work, play, and capture moments to behold and cherish. A home where every view is a view to live for." />

				<SliderSection :image="dubaiCreekImg" />
			</div>

			<div class="content" id="cove">
				<DetailsCard :image="cove" title="creek rise"
					desc="At Dubai Creek Harbour, you will experience more of what really matters. More laughs shared with friends More memories made. A thriving community to live, work, play, and capture moments to behold and cherish. A home where every view is a view to live for." />

				<SliderSection :image="park" />
			</div>

			<div class="content" id="gate">
				<DetailsCard :image="gate" title="creek rise"
					desc="At Dubai Creek Harbour, you will experience more of what really matters. More laughs shared with friends More memories made. A thriving community to live, work, play, and capture moments to behold and cherish. A home where every view is a view to live for." />

				<SliderSection :image="urbana" />
			</div>
		</div>



	</section>
</template>

<style lang="scss" scoped>
.details {
	display: flex;
	justify-content: space-between;
	gap: 20px;


	.navigation {
		margin-top: 10px;
		padding: 30px;
		width: 310px;
		height: 310px;
		background: #FFFFFF;
		border: 1px solid rgba(0, 0, 0, 0.05);
		box-shadow: 0px 0px 14px 3px rgba(0, 0, 0, 0.03);

		position: sticky;
		top: 20px;

		.lists {
			.title {
				font-family: 'Lato';
				font-style: normal;
				font-weight: 500;
				font-size: 20px;
				line-height: 24px;
				text-transform: uppercase;
				color: #071C35;
			}

			.wrapper {
				margin-top: 15px;
				display: flex;
				flex-direction: column;
				gap: 12px;
			}
		}

		.projects {
			margin-top: 20px;


			.title {
				font-family: 'Lato';
				font-style: normal;
				font-weight: 500;
				font-size: 20px;
				line-height: 24px;
				/* identical to box height, or 120% */
				text-transform: uppercase;

				color: #071C35;
			}

			.item {
				margin-top: 10px;
				display: block;
				font-family: 'Lato';
				font-style: normal;
				font-weight: 400;
				font-size: 16px;
				line-height: 19px;
				text-transform: uppercase;
				color: #777;
			}

			.active {
				font-weight: 500;
				color: #071C35;

			}
		}
	}

	.projects-content {
		display: flex;
		flex-direction: column;
		gap: 107px;

		.content {
			position: relative;
			padding: 25px;
			border: 1px solid rgba(7, 28, 53, 0.1);

			display: flex;
			flex-direction: column;
			gap: 50px;
		}
	}

}
</style>