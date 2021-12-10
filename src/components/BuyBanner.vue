<template>
	<section>
		<div class="buy-banner">
			<div class="wraper">
				<h2 class="buy-banner__title" >"I've failed over and over again in my life. And that is why i sycceed."</h2>
				<div class="centered-curved-line"><span class="curved-line banner-line"></span></div> 
				<p class="buy-banner__txt"> Quibusdam dignissimos dolores architecto pariatur quia consectetur, nobis voluptatibus quis ex numquam molestiae dolorum laborum aperiam obcaecati harum dolor dolore nihil delectus.</p>
				<button class="btn buy-banner-btn">Buy Avada Today ></button>
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
		background-image: url('../assets/banner2-2x.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		
		.buy-banner{
			padding: 150px 0;
			display: flex;
			justify-content: center;
			background: #000000;
			background: -webkit-linear-gradient(to top, #000000 2%, #ffffff00 100%);
			background: -moz-linear-gradient(to top, #000000 2%, #ffffff00 100%);
			background: linear-gradient(to top, #000000 2%, #ffffff00 100%);
			.wraper{
				text-align: center;
				max-width: 780px;
				.buy-banner__title{
					font-size: 2.5rem;
					color: $white;
				}
				.buy-banner__txt{
					color: $white;
					margin-bottom: 30px;

					
				}

				.buy-banner-btn{
					padding: 20px 40px;
					background: $dodgerBlue;
					color: $white;

				}
				.centered-curved-line{
					display: flex;
					justify-content: center;
				}	
			}
		}
	}
</style>
