<template>
	<section>
		<div class="container">
			<div class="logo">
				<img src="../assets/logo-200x34.png" alt="">
			</div>
			<nav class="nav-bar">
				<ul>
					<li v-for="(elem,index) in headerData" :key = "index">
						{{elem.name}}
						<span v-show = elem.new class="new">new</span>
					</li>
				</ul>
						<button class="btn header-button">Schedule a workout</button>
						<button class="search"><i class="fas fa-search"></i></button>
						<button class="cart"><i class="fas fa-shopping-cart"></i></button>
				
			</nav>

		</div>
	</section>
</template>

<script>
export default {
  
  props: {
    headerData:Array
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
				.header-button{
								padding: 15px 30px;
								background: $dodgerBlue;
								color: $white;
								transition: linear 0.2s;
								&:hover{
									background: $monza;
								}
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
								margin: 0 20px;

								
							}
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
							
						}
				}
			}
		
		}
	}
</style>
