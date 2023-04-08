<script setup lang="ts">
import TopProject from '../../shared/top-project/index.vue'

// import background from '../../../assets/img/sale-image.png'
import project1 from '../../../assets/img/content/top-projects/1.jpg'
import project2 from '../../../assets/img/content/top-projects/2.jpg'
import project3 from '../../../assets/img/content/top-projects/3.jpg'


</script>

<template>
	<section class="top-projects">
		<h2 class="title">top projects</h2>
		<div class="projects">
			<TopProject :image="project1" :title="`creek rise`" :info="`FROM AED 2,288,888`" />
			<TopProject :image="project2" :title="`EXPO GOLF VILLAS 6`" :info="`FROM AED 2,288,888`" />
			<TopProject :image="project3" :title="`HILLS PARK`" :info="`FROM AED 2,288,888`" />

		</div>
	</section>
</template>

<style lang="scss" scoped>
.top-projects {
	padding-top: 136px;

	.title {
		font-family: 'Alethia Pro';
		font-style: normal;
		font-weight: 400;
		font-size: 54px;
		line-height: 40px;
		/* identical to box height, or 74% */
		text-align: center;
		text-transform: uppercase;

		color: #071C35;

	}

	.projects {
		padding-top: 67px;

		display: flex;

		justify-content: space-between;
		gap: 20px;
	}
}
</style>w