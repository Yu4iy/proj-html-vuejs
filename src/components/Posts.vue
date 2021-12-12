<template>
	<section>
		<div class="container">
			<div class="title">
				<h2 class="title__txt">Featured playlist</h2>
				<button class="title__show-btn">view all videos ></button>
			</div>
		</div>
		<div class="cards">

			<div class="container">
				<div class="card">
						<div class="card__img">
							<img src="../assets/video7-2x.jpg" alt="">
						</div>
						
						<h3 class="card__title">Thighs & glute workout</h3>
						<div class="card__date">Increase your mobility</div>
				</div>

				<div class="card">
						<div class="card__img">
							<img src="../assets/video2-2x.jpg" alt="">
						</div>
						
						<h3 class="card__title">Thighs & glute workout</h3>
						<div class="card__date">Increase your mobility</div>
				</div>

				<div class="card">
						<div class="card__img">
							<img src="../assets/video7-2x.jpg" alt="">
						</div>
						
						<h3 class="card__title">Thighs & glute workout</h3>
						<div class="card__date">Increase your mobility</div>
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

.cards{
        padding: 0 0 130px 0;

    >div{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    .card{
		display: flex;
		text-align: center;
		flex-direction: column;
		max-width: 400px;
		margin: 10px 10px;
		.card__img{
				position: relative;
				display: flex;
				justify-content: center;
				align-items: center;
				img{
					max-height: 250px;
					object-fit: cover;
					width: 100%;
					border-radius: 5px;
	
				}

			}
		.card__title{
			text-align: start;
			margin: 35px 0 10px 0;
		}
		.card__date{
			text-align: start;
		}	

    }
  }


	.title{
			display: flex;
			justify-content: space-between;
			margin: 100px 0 40px 0 ;
	}

</style>
