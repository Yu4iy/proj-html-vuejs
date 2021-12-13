<template>
	<section>
		<div class="container">
				<div class="column column-info">
					<img class="logo" src="../assets/logo-200x34.png" alt="">
					<p>{{footerData.text}}</p>
					<div class="icons">
						<a :href="footerData.f"><i class="fab fa-facebook-f"></i></a>
						<a :href="footerData.f"><i class="fab fa-twitter"></i></a>
						<a :href="footerData.f"><i class="fab fa-youtube"></i></a>
						<a :href="footerData.f"><i class="fab fa-instagram"></i></a>
						<a :href="footerData.f"><i class="fab fa-linkedin-in"></i></a>	
					</div>
				</div>
				
				<div class=" column column-posts">
					<h2>Recent posts</h2>
					<ul>
						<li><i class="fas fa-angle-right"> </i> The best protein shake</li>
						<li><i class="fas fa-angle-right"> </i> The best protein shake</li>
						<li><i class="fas fa-angle-right"> </i> The best protein shake</li>
						<li><i class="fas fa-angle-right"> </i> The best protein shake</li>
						<li><i class="fas fa-angle-right"> </i> The best protein shake</li>
					</ul>
				</div>

				<div class="column column-address">
					<h2>Address</h2>
					<address>
						<div class="address">{{footerData.address}}</div>
						<div class="mobile">Mobile: <a href="tel:1.800.000.000.0000">{{footerData.mobile}}</a></div>
						<div class="mail">Email: <a href="mailto:info@your-company.com">{{footerData.mail}}</a></div>
					</address> 	
				</div>
		</div>
		<hr>
		<div class="copy">
			&copy; Copyright
		</div>
	</section>
</template>

<script>
export default {

  props: {
	footerData:Object
  }
}
</script>


<style scoped lang="scss">
@import "@/styles/variables.scss";
	section{
		background: $codGray;

		.container{
			padding: 130px 100px ;
			display: flex;
			flex-wrap: wrap;
			justify-content: center;
			align-items: baseline;
			color: #fff;

			.column{
				display: flex;
				flex-direction: column;
				justify-content: center;
				align-items: center;
				text-align: center;
				width: calc(100% / 3);
				min-width: 350px;
				padding: 5px 15px;
					@media screen and (max-width: 1250px) {
						&{
							margin-bottom: 50px ;
						}
					}
				
				h2{
					text-transform: uppercase;
					font-size: 15px;
					margin-bottom: 40px;
					@media screen and (max-width: 1250px) {
						&{
							margin-bottom: 10px ;
						}
					}
					
				}
			}
			.column-info{

				p{
					color: $silver;
					line-height: 1.25rem;
					margin: 50px 0;
					@media screen and (max-width: 1250px) {
						&{
							margin: 10px 0;
						}
					}
				}
				i{
					margin-left: 15px;
					transition: linear 0.2s;
					&:last-child{
						margin: none;
					}
					&:hover{
						color: $white;
					}
				}
			}
			.column-posts{
				order: 2;
				ul{
					li{
						margin-bottom: 30px;
					}
				}
			}
			.column-address{
				.address{
					color: $silver;
					margin-bottom: 25px;
				}
				a{
					color: $white;
					line-height: 25px;
				}

			}
			address{
				font-style: normal ;
			}
			
			a{
				color: $monza;
			}
		}
		.copy{
			padding: 50px 0;
			text-align: center;
			color: $white;
		}

	}
</style>
