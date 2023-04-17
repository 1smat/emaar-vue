<script setup lang="ts">
import payment from '../../../assets/img/content/options/payment.png'
import more from '../../../assets/img/content/options/more.png'

</script>


<template>
	<section class="options">
		<div class="card">
			<div class="image">
				<img :src="payment" alt="Option" />
			</div>
			<div class="content">
				<h2 class="title">payment option</h2>
				<hr class="line" />
				<p class="desc">Emaar properties offer various payment options to help make your property purchase as
					stress-free as possible. Some project have up to 3 Years payment plan and we also offer mortgage option
					for
					ready units. Click "Enquire Now" below to get more information about payment options available for your
					purchase.</p>
				<button class="button">enquire now</button>
			</div>
		</div>

		<div class="card card-reverse">
			<div class="image">
				<img :src="more" alt="Option" />
			</div>
			<div class="content">
				<h2 class="title">payment option</h2>
				<hr class="line" />
				<p class="desc">Emaar properties offer various payment options to help make your property purchase as
					stress-free as possible. Some project have up to 3 Years payment plan and we also offer mortgage option
					for
					ready units. Click "Enquire Now" below to get more information about payment options available for your
					purchase.</p>
				<button class="button">enquire now</button>
			</div>
		</div>
	</section>
</template>


<style lang="scss" scoped>
.options {
	display: flex;
	flex-direction: column;
	gap: 150px;
	padding-top: 180px;

	.card {
		position: relative;
		display: flex;
		background-image: none;
		background-attachment: fixed;
		height: 500px;


		.image {
			background-image: url('../../../assets/img/content/options/payment.png');
			background-attachment: fixed;
			background-position: center;
			background-size: cover;
			background-repeat: no-repeat;
		}

		.content {
			position: absolute;
			top: 213px;
			padding: 50px;
			right: 0;
			width: 610px;
			background: rgba(255, 255, 255, 0.85);
			box-shadow: 0px 20px 30px rgba(0, 0, 0, 0.07);
			backdrop-filter: blur(1.5px);

			.title {
				font-family: 'Alethia Pro';
				font-style: normal;
				font-weight: 400;
				font-size: 50px;
				line-height: 120%;
				text-transform: uppercase;
				color: #071C35;
			}

			.line {
				height: 2px;
				width: 236px;
				background: #071C35;
				opacity: 0.1;
			}

			.desc {
				margin-top: 30px;
				font-family: 'Lato';
				font-style: normal;
				font-weight: 300;
				font-size: 16px;
				line-height: 24px;
				color: #071C35;
			}

			.button {
				margin-top: 26px;
				padding: 12px 30px;
				font-family: 'Lato';
				font-style: normal;
				font-weight: 400;
				font-size: 14px;
				line-height: 17px;
				text-transform: uppercase;
				color: #071C35;

				border: 1px solid rgba(7, 28, 53, 0.15);
			}
		}



	}

	.card-reverse {
		position: relative;
		display: flex;
		flex-direction: row-reverse;

		.content {
			position: absolute;
			top: 213px;
			padding: 50px;
			left: 0;
			width: 610px;
			background: rgba(255, 255, 255, 0.85);
			box-shadow: 0px 20px 30px rgba(0, 0, 0, 0.07);
			backdrop-filter: blur(1.5px);
		}
	}
}
</style>