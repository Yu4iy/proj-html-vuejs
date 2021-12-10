<template>
	<section>
		<div class="form-banner">
			<div class="container">
				<div class="wraper">
					<h2 class="form-banner__subtitle">Join our mailing list today</h2>
					<h3 class="form-banner__title">Insider offers & flash salesin your inbox every week</h3>
					<span class="curved-line quote-line"></span>
					<div class="form-banner__form">
						<input class="btn" type="text">
						<button class="btn" type="submit">Subscribe</button>
					</div>
					<p class="form-banner__txt">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Officiis, beatae! Vero assumenda sapiente non adipisci, error debitis </p>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {

  props: {
  
  }
}
</script>


<style scoped lang="scss">
	@import "@/styles/variables.scss";
	section{
		background: url('../assets/banner1-2x.jpg');
		background-size: cover;
		.form-banner{
			background: linear-gradient(to right, #000000, #000000, #000000ce, #b9b9b900, #ffffff00);
			padding: 50px 0 100px;
			.wraper{
				max-width: 750px;
				.form-banner__subtitle{
					font-size: 1.375rem;
					color: $monza;
				}
				.form-banner__title{
					font-size: 2.8125rem;
					color: $white;
					margin: 30px 0;
				}
				.form-banner__form{
					display: flex;
					margin: 40px 0 ;

					input{
						flex-grow: 1;
						max-width: 580px;
						height: 55px;

					}
					button{
						flex-grow: 1;
						height: 55px;
						padding: 20px 0;
						max-width: 270px;

						color: $white;
						background-color: $dodgerBlue;
						margin: 0 0 0 35px;
					}
				}
					.form-banner__txt{
						color: $silver;
					}
			}
			
		}
		
	}
</style>
