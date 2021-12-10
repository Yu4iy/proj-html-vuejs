<template>
	<section>
			<div class="container">
				<div class="title">
					<h2 class="title__txt">Latest articles</h2>
					<button class="post-show-btn">read all articles ></button>
				</div>
				<div class="posts">
					<div class="card">
						<div class="card__img">
							<img src="../assets/video7-2x.jpg" alt="">
						</div>
						
						<h3 class="card__title">Thighs & glute workout</h3>
						<div class="card__date">Increase your mobility</div>
					</div>
					<div class="card">
						<div class="card__img">
							<img class="card__img" src="../assets/video2-2x.jpg" alt="">
						</div>				
						<h3 class="card__title">Thighs & glute workout</h3>
						<div class="card__date">Increase your mobility</div>
					</div>
					<div class="card">
						<div class="card__img">
							<img class="card__img" src="../assets/video9-2x.jpg" alt="">
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
	section{
		padding: 100px 0; 
	}
	.title{
			display: flex;
			justify-content: space-between;
			.post-show-btn{
				background: none;
				border: none;
			}
	}
	.posts{
		display: flex;
		.card{
			width: 33.3333%;
			margin: 25px;
			.card__img{
				position: relative;
				img{
					max-height: 250px;
					object-fit: cover;
					width: 100%;
					border-radius: 5px;
	
				}

			}
	
		}
	}
</style>
