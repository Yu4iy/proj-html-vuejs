<template>
	<section>
		<div class="container">
			<div class="logo">
				<img src="../assets/logo-200x34.png" alt="">
			</div>
			<nav class="nav-bar">
				<ul>
					<li>
						Home
					</li>
					<li>
						Sevices
					</li>
					<li>
						About
					</li>
					<li>
						Videos
					</li>
					<li>
						Blog
					</li>
					<li>
						Store
						<span class="new">new</span>
					</li>
					<li>
						<button class="btn header-button">Schedule a workout</button>
					</li>
					<li>
						<button class="cart"><i class="fas fa-shopping-cart"></i></button>
					</li>
					<li>
						<button class="search"><i class="fas fa-search"></i></button>
					</li>
				</ul>
				
				
			</nav>

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
		padding: 30px 0;
		
		>div{
			display: flex;
			align-items: center;
			justify-content: space-between;
			.nav-bar{
				display: flex;
					ul{
						display: flex;
						align-items: center;

						li{
							color: $silver;
							margin-right: 40px;
							.new{
								color: $codGray;
								background: $yellow;
								padding: .625rem .5rem;
								border-radius: .125rem;
							}
							.header-button{
								padding: 15px 30px;
								background: #4154fe;
								color: $white;
							}
							.cart{
								color: $silver;
								background: none;
								border: none;

							}
							.search{
								color: $silver;
								background: none;
								border: none;
								
							}
						}
				}
			}
		
		}
	}
</style>
