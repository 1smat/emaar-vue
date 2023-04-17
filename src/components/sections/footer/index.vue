<script setup lang="ts">
import Container from '../../container/Container.vue'
import women from '../../../assets/img/content/footer/women.png'
import logo from '../../../assets/img/logo-shape.png'
import telegram from '../../../assets/img/telegram.svg'
import whatsapp from '../../../assets/img/whatsapp.svg'

</script>

<template>
	<footer class="footer">
		<Container>
			<div class="wrapper">
				<div class="content">
					<h2 class="title">SPEAK TO A SPECIALIST</h2>
					<hr class="line" />
					<div class="desc">
						<div class="subtitle">
							<span class="green"></span>
							<span class="online">We are Online</span>
						</div>
						<div class="info">
							Contact us below to get limited availability, payment plan and to book a unit.
						</div>
					</div>
					<form action="" class="form">
						<input type="text" class="input" placeholder="Your name" />
						<input type="text" class="input" placeholder="Your email" />
						<input type="text" class="input" placeholder="Phone number" />
						<input type="submit" class="input submit" value="REQUEST TO CALL" />

					</form>
				</div>
			</div>

		</Container>
		<div class="bottom">
			<Container>
				<div class="wrapper">
					<div class="women">
						<img :src="women" alt="women" class="women-img" />
					</div>
					<div class="contacts">
						<div>
							<ul class="links">
								<li class="link-item">
									<a href="#" class="link">top projects</a>
								</li>
								<li class="link-item">
									<a href="#" class="link">community</a>
								</li>
								<li class="link-item">
									<a href="#" class="link">payment option</a>
								</li>
							</ul>
							<ul class="links social">
								<li class="link-item">
									<a href="#" class="link">971 56XXX-XX-XX SHOW</a>
								</li>
								<li class="link-item">
									<a href="#" class="link">
										<span>telegram</span> <img :src="telegram" alt="telegram" />
									</a>
								</li>
								<li class="link-item">
									<a href="#" class="link">
										<span>whatsapp </span><img :src="whatsapp" alt="whatsapp" />
									</a>
								</li>
							</ul>
						</div>
						<div class="logo">
							<img :src="logo" alt="logo emaar" />
						</div>
					</div>
				</div>
			</Container>

		</div>
	</footer>
</template>

<style lang="scss" scoped>
.footer {
	margin-top: 210px;
	position: relative;

	.wrapper {
		display: flex;
		justify-content: flex-end;
	}

	.content {
		.title {
			font-family: 'Alethia Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 44px;
			line-height: 40px;
			text-transform: uppercase;
			color: #071C35;
		}

		.line {
			margin-top: 7px;
			width: 868px;
			height: 18px;
			background: #D9D9D9;
		}

		.desc {
			margin-top: 37px;
			display: flex;
			align-items: center;

			.subtitle {
				display: flex;
				align-items: center;

				.online {
					position: relative;
					left: -30px;
					font-family: 'Lato';
					font-style: normal;
					font-weight: 500;
					font-size: 16px;
					line-height: 24px;
					color: #071C35;
				}

				.green {
					display: inline-block;
					border-radius: 50%;
					height: 50px;
					width: 50px;
					background: #85DF99;
				}
			}

			.info {
				font-family: 'Lato';
				font-style: normal;
				font-weight: 300;
				font-size: 16px;
				line-height: 24px;
				color: #777777;
			}
		}

		.form {
			margin-top: 60px;
			display: flex;
			align-items: center;
			gap: 20px;

			.input {
				border-bottom: 1px solid rgba(7, 28, 53, 0.1);
				padding: 11px;
			}

			.submit {
				border: 1px solid rgba(7, 28, 53, 0.15);
				padding: 11px 44px;
			}
		}
	}

	.bottom {
		margin-top: 50px;
		height: 237px;
		background: #071C35;
		position: relative;
		padding-top: 80px;
		display: flex;
		justify-content: flex-end;

		.wrapper {
			position: relative;

			.women {
				position: absolute;
				bottom: -47px;
				left: 0;

			}
		}

		.contacts {
			display: flex;
			justify-content: space-between;
			width: 868px;

			.links {
				display: flex;
				gap: 30px;

				.link-item {
					.link {
						font-family: 'Lato';
						font-style: normal;
						font-weight: 400;
						font-size: 14px;
						line-height: 24px;
						text-transform: uppercase;
						color: #fff;
					}
				}
			}

			.social {
				gap: 50px;
				margin-top: 30px;

				.link-item {
					.link {
						display: flex;
						gap: 10px;
						align-items: center;
					}
				}
			}
		}
	}
}
</style>