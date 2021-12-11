<template>
	<section>
		<div class="container">
				<div class="column column-info">
					<img class="logo" src="../assets/logo-200x34.png" alt="">
					<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis, sapiente ea assumenda voluptate hic perferendis magnam</p>
					<div class="icons">
						<i class="fab fa-facebook-f"></i>
						<i class="fab fa-twitter"></i>	
						<i class="fab fa-youtube"></i>
						<i class="fab fa-instagram"></i>
						<i class="fab fa-linkedin-in"></i>	
					</div>
				</div>
				
				<div class=" column column-posts">
					<h2>Recent posts</h2>
					<ul>
						<li>>The best protein shake</li>
						<li>>The best protein shake</li>
						<li>>The best protein shake</li>
						<li>>The best protein shake</li>
						<li>>The best protein shake</li>
					</ul>
				</div>

				<div class="column column-adress">
					<h2>Recent posts</h2>
					<address>
						<div class="adress">4746 Tipple Road Micighan 48449</div>
						<div class="mobile">Mobile:<a href="tel:+74951234567">1.800.000.000.0000</a></div>
						<div class="mail">Email:<a href="mailto:info@your-company.com">info@your-company.com</a></div>
						
						
					</address> 	
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
		background: $codGray;
		padding-top: 130px ;
		padding-bottom: 100px ;

		>div{
			display: flex;
				align-items: baseline;
				color: #fff;

			.column{
				display: flex;
				flex-direction: column;
				justify-content: center;
				align-items: center;
				text-align: center;
				width: calc(100% / 3);
				padding: 5px 15px;
				h2{
					text-transform: uppercase;
					font-size: 15px;
					margin-bottom: 40px;
				}
			}
			.column-info{
				p{
					color: $silver;
					line-height: 1.25rem;
					margin: 50px 0;
				}
				i{
					margin-left: 15px;
					&:last-child{
						margin: none;
					}
				}
			}
			.column-posts{
				ul{
					li{
						margin-bottom: 30px;
					}
				}
			}
			.column-adress{
				.adress{
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
			
			.icons{
				color: $monza;
			}
		}

	}
</style>
