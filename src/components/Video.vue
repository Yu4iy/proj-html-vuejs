<template>
<section>
	<div class="top">
			<div class="poster">
				<img src="../assets/service.jpg" alt="">
				<a class="poster__play play" href=""><i class="fas fa-play"></i></a>
			</div>
			<div class="yt-ref">
				<h2 class="yt-ref__desc">Tune up your workouts</h2>
				<h3 class="yt-ref__title">Yhe best health & fitness advice online</h3>
				<div class="yt-ref__profile">
					<img src="../assets/YTlogo.jpg" alt="">
					<div>
						<h4 class="yt-ref__profile-name">ThemeFusion</h4>
						<div class="yt-ref__subscribe">
							<a href="">
								<i class="fab fa-youtube"></i>
								YouTube
							</a>
							<span>
								999+
							</span>
						</div>
					</div>
				</div>
				<p class="yt-ref__txt">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ex, ut nostrum at alias dolor quaerat optio possimus </p>
				<button class="btn yt-ref__btn"><i class="fab fa-youtube"></i> Visit my YouTube channel</button>
			</div>
	</div>
		
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
								<img class="card__img" src="../assets/video2-2x.jpg" alt="">
								<a class="card__play play" href=""><i class="fas fa-play"></i></a>
							</div>		
							<h3 class="card__title">Thighs & glute workout</h3>
					<div class="card__subtitle">Increase your mobility</div>
			</div>

			<div class="card">
					<div class="card__img">
								<img class="card__img" src="../assets/video7-2x.jpg" alt="">
								<a class="card__play play" href=""><i class="fas fa-play"></i></a>
							</div>		
							<h3 class="card__title">Thighs & glute workout</h3>
					<div class="card__subtitle">Increase your mobility</div>
			</div>

			<div class="card">
					<div class="card__img">
								<img class="card__img" src="../assets/video9-2x.jpg" alt="">
								<a class="card__play play" href=""><i class="fas fa-play"></i></a>
							</div>		
							<h3 class="card__title">Thighs & glute workout</h3>
					<div class="card__subtitle">Increase your mobility</div>
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
        padding: 100px 0 160px 0;

    >div{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    .card{
		display: flex;
		align-items: center;
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
					border-bottom-right-radius: 30px;
	
				}

				.card__play{
					width: 50px;
					height: 50px;
					font-size: 10px;
					position: absolute;
					&:hover{
						color: $monza;
					}
				}
			}

    }
  }



	.top{
			display: flex;
			flex-wrap: wrap;
			.poster{
				display: flex;
				justify-content: center;
				align-items: center;
				width: 50%;
				position: relative;
				.poster__play{
					position: absolute;
					width: 100px;
					height: 100px;
					font-size: 20px;
					&:hover{
						color: $monza;
					}
					
				}
				img{
					margin: -50px 0 0 0;
					border-bottom-right-radius: 50px;
				}
			}
			.yt-ref{
				width: 50%;
				padding: 130px 100px 130px;
				.yt-ref__desc{
					font-size: 1.25rem;
					color: $dodgerBlue;
				}
				.yt-ref__title{
					font-size: 2.8125rem;
					margin: 50px 0 0 0;
				}
				.yt-ref__profile{
					display: flex;
					align-items: center;
					margin: 50px 0 40px 0;
					img{
						margin-right: 15px;
					}
					div{
						.yt-ref__profile-name{
							font-size: .625rem;
							color: gray;
							
						}
						.yt-ref__subscribe{
							margin: 10px 0 0 0;
							a{
								background-color: red;
								border: 1px solid red;
								padding: 5px 8px;
								color: white;
								
							}
							span{
								background-color: #fafafa;
								border: 1px solid lightgray;
								border-left: none;
								padding: 5px 8px;
								color: gray;

							}

						}
					}
					
				}
				.yt-ref__txt{
					color: gray;

					}
				.yt-ref__btn{
					padding: 20px 40px;
					background: red;
					color: #fff;
					margin: 35px 0 0 0;
					transition: linear 0.2s;
					&:hover{
						background: rgb(189, 12, 12);
					}
				}

			}
		}

		.title{
				display: flex;
				justify-content: space-between;
				margin: 130px 0 0 0 ;
				.title__show-btn{
					border: none;
					background: none;
				}
		}
	
</style>
