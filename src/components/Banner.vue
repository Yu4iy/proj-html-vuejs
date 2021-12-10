<template>
	<section>
		<div class="banner">
			<div class="container">
				<h3 class="banner__txt">Certified fitness professional</h3>
				<h2 class="banner__title">Take controle of your health</h2>
				<span class="curved-line banner-line"></span>
				<p class="banner__subtitle"> Voluptatem iure eius quam enim, praesentium animi sint deserunt ipsum a, blanditiis</p>
				<a class="btn banner__visit"><i class="fab fa-youtube"></i> Visit my YouTube channel</a>
				<button class="btn banner__buy">Buy Avada today <i class="fas fa-arrow-right"></i></button>
				<a class="banner__more" href=""><i class="fas fa-play"></i></a>

			</div>
		</div>

		<div class="banner-cards">
			<div class="container">
				<div class="banner-card">
					
					<div class="banner-card__img">
						<img src="../assets/card1.jpg" alt="">
					</div>
					<div class="info">
						<span class="curved-line info-line"></span>
						<h4 class="info__title">Crossfit workout</h4>
						<h5 class="info__subtitle">Push your limits</h5>
					</div>
					
				</div>
				<div class="banner-card">
					<div class="banner-card__img">
						<img src="../assets/card2.jpg" alt="">
					</div>
					<div class="info">
						<span class="curved-line info-line"></span>
						<h4 class="info__title">Crossfit workout</h4>
						<h5 class="info__subtitle">Push your limits</h5>
					</div>
				</div>
				<div class="banner-card">
					<div class="banner-card__img">
						<img src="../assets/card3.jpg" alt="">
					</div>
					<div class="info">
						<span class="curved-line info-line"></span>
						<h4 class="info__title">Crossfit workout</h4>
						<h5 class="info__subtitle">Push your limits</h5>
					</div>
				</div>
			</div>
			<div class="quote">
					<p class="quote__txt">"  Senetur accusantium? Consequuntur eius suscipit dolores id, sequi aperiam similique asperiores mollitia, nemo sed provident dicta dolor. Voluptatum, fugiat? "</p>
					<span class="curved-line quote-line"></span>
					<div class="profile">
						<img class="profile__img" src="../assets/avatar-1-2x.jpg" alt="">
						<h6 class="profile__name">Brad Johnson</h6>
						<span class="profile__place">Las Vegas</span>
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
		background-image: url('../assets/ban.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		.banner{
			position: relative;
			padding: 150px 0;
			background-image: linear-gradient(to right, #000000, #000000, #00000090, #b9b9b900, #ffffff00);
			.banner__txt{
				color: $monza;
				font-size: 1.25rem;
			}
			.banner__title{
				color: $white;
				font-size: 3.125rem;
				margin: 35px 0;

			}
			.banner__subtitle{
				color: $silver;
				font-size: 16px;
				margin: 35px 0;
			}
			.banner__visit{
				padding: 15px 30px;
				background: $dodgerBlue;
				color: $white;
				margin-right: 15px;
			}
			.banner__buy{
				padding: 15px 30px;
				background: transparent;
				color: $white;
				border: 3px solid rgba(128, 128, 128, 0.435);
			}
			.banner__more{
				position: absolute;
				display: flex;
				justify-content: center;
				align-items: center;
				width: 100px;
				height: 100px;
				background-color: $white;
				color: $dodgerBlue;
				border-radius: 50% ;
				font-size: 20px;
				top: 50%;
				right: 20%;
				transform: translatey(-50%);
			
			}

		}
		.banner-cards{
			height: 100vh;
			background: #0818E4;
			background: -webkit-linear-gradient(to bottom right, #0818E4 0%, #CE0113 100%);
			background: -moz-linear-gradient(to bottom right, #0818E4 0%, #CE0113 100%);
			background: linear-gradient(to bottom right, #0818E4 0%, #CE0113 100%);
			>div{
				display: flex;
			}
			.banner-card{
				width: calc(100% / 3);
				max-height: 380px;
				margin: -70px 50px 0 0;
				z-index: 2;
				border-radius: 5;
				border-bottom-right-radius: 70px;
				overflow: hidden;
				position: relative;
				transition: linear 0.2s;
				box-shadow: 0px 2px 3px -1px #000000, 2px 1px 1px 3px rgba(0,0,0,0);

					&:hover{
						transform: scale(1.1);
						-webkit-box-shadow: 0px 10px 13px -7px #000000, 10px 5px 4px 14px rgba(0,0,0,0); 
						box-shadow: 0px 10px 13px -7px #000000, 10px 5px 4px 14px rgba(0,0,0,0);
					}
				.banner-card__img{
					
					&:before {
					content: ' ';
					position: absolute;
					top: 0;
					bottom: 0;
					right: 0;
					left: 0;
					width: 100%;
					height: calc(100%);
					background: #000000;
					background: -webkit-linear-gradient(to top, #00000090 0%, #ffffff02 100%);
					background: -moz-linear-gradient(to top, #0000008d 0%, #ffffff00 100%);
					background: linear-gradient(to top, #0000008b 0%, #ffffff00 100%);
				
				}
				}
				.info{
					position: absolute;
					z-index: 3;
					bottom: 2.5rem;
					left: 2.5rem;

					.info-line{
						width: 60px;
						&::before{
							text-decoration-color:$white;
							font-size: 28px
							}
					}
					.info__title{
						color: $white;
						font-size: 1.5625rem;
					}
					.info__subtitle{
						color: $yellow;
						font-size: 1.25rem;
					}
				}
			}
		}
		.quote{
			margin: 130px 0 0 0 ;
			display: flex;
			align-items: center;
			justify-content: center;
			flex-direction: column;
			text-align: center;
			width: 100%;
			.quote__txt{
				font-size: 2.25rem;
				max-width: 1000px;
				color: $white;
				font-weight: 600;
				margin:  0 0 10px 0;
			}
			.profile{
				display: flex;
				align-items: center;
				.profile__img{
					border-radius: 50%;
					width: 55px;
				}
				.profile__name{
					font-size: .9375rem;
					margin: 0 15px;
					color: $white;

				}
				.profile__place{
					color: $silver;
				}

			}

			
		}
	}
			
</style>
