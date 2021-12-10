<template>
	<section>
		<div class="container">
			<div class="other-services">
			

				<div class="services-card">
					<img class="services-card__logo" src="../assets/service-card3.png" alt="">
					<span class="curved-line quote-line"></span>
					<p class="services-card__txt">Lorem adipisicing elit ipsum amet consectetur adipisicing elit ipsum dolor sit amet consectetur adipisicing elit. , cumque quod?</p>
					<button class="services-card__btn">Visit Yoga Studio ></button>
				</div>

				<div class="services-card">
					<img class="services-card__logo" src="../assets/service-card2.png" alt="">
					<span class="curved-line quote-line"></span>
					<p class="services-card__txt">Lorem adipisicing elit ipsum amet consectetur adipisicing elit ipsum dolor sit amet consectetur adipisicing elit. , cumque quod?</p>
					<button class="services-card__btn">Visit Yoga Studio ></button>
				</div>
				
				<div class="services-card">
					<img class="services-card__logo" src="../assets/service-card3.png" alt="">
					<span class="curved-line quote-line"></span>
					<p class="services-card__txt">Lorem adipisicing elit ipsum amet consectetur adipisicing elit ipsum dolor sit amet consectetur adipisicing elit. , cumque quod?</p>
					<button class="services-card__btn">Visit Yoga Studio ></button>
				</div>
				
				<div class="services-card">
					<img class="services-card__logo" src="../assets/service-card2.png" alt="">
					<span class="curved-line quote-line"></span>
					<p class="services-card__txt">Lorem adipisicing elit ipsum amet consectetur adipisicing elit ipsum dolor sit amet consectetur adipisicing elit. , cumque quod?</p>
					<button class="services-card__btn">Visit Yoga Studio ></button>
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
		padding: 100px 0;
	}
	.other-services{
		display: flex;
		.services-card{
			width: calc(100% / 4);
			margin: 15px 15px;
			padding: 0 15px;
			display: flex;
			flex-direction: column;
			align-items: center;
		}
		.services-card__txt{
			text-align: center;
			font-size: .75rem;
			line-height: 1.35rem;
		}
		.services-card__btn{
			margin: 40px 0 0 0 ;
			border: none;
			background: none;
		}
	}
</style>
