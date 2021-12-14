<template>
	<section>
		<div class="container">
			<div class="logo">
				<img class="logo-full" src="../assets/logo-200x34.png" alt="">
				<img class="logo-mobile" src="../assets/logo-mobile.png" alt="">
			</div>
			<nav class="nav-bar" >
				<ul  >
					<li  v-for="(elem,index) in headerData" :key = "index">
						{{elem.name}}
						<span v-show = elem.new class="new">new</span>
					</li>
				</ul>
				<div v-if="display" class="hamburger-menu" >
					<ul class="hamburger-menu__ul">
						<li class="hamburger-menu__item" v-for="(elem,index) in headerData" :key = "index">
							{{elem.name}}
							<span v-show = elem.new class="new">new</span>
						</li>
					</ul>
					<a @click="test()" href="#" class="close">
						<i class="fas fa-times"></i>
					</a>
				</div>


				<button class="btn header-button">Schedule a workout</button>
				<button class="search"><i class="fas fa-search"></i></button>
				<button class="cart"><i class="fas fa-shopping-cart"></i></button>
				<button @click="test()" class="burger"><i class="fas fa-bars"></i></button>
						
				
			</nav>

		</div>
	</section>
</template>

<script>
export default {
  data(){
	return {
      display:false,

    };
  },
  props: {
    headerData:Array
  },
	methods:  {
		test(){
			this.display = !this.display
		}
  }
}

</script>


<style scoped lang="scss">
	@import "@/styles/variables.scss";
	

	.logo-mobile{
				display: none;
			}	
	
	@media screen and (max-width: 1150px) {
		.logo-full {
			display: none;
		}
		.logo-mobile{
			display: inline;
		}
  }
	

	section{
		background: $codGray;
		padding: 30px 20px;
		
		>div{
			display: flex;
			align-items: center;
			justify-content: space-between;
			
			.nav-bar{
				display: flex;
				.hamburger-menu{
					background: $codGray;
					position: absolute;
					top: 0;
					left: 0;
					padding: 20px;
					width: 100%;
					height: 100%;
					min-width: 100vw;
					min-height: 100vh;
					z-index: 200;
					position: fixed;
					
						.hamburger-menu__ul{
						display: flex;
						flex-direction: column;
						align-items: center;
						justify-content: center;
						height: 100%;

						.hamburger-menu__item{
							margin: 30px 0;
							color: $white;
							font-size: 2rem;
							font-weight: 700;
							&:hover{
								color: $dodgerBlue;
							}
						}
					}
				.close{
					position: absolute;
					top: 20px;
					right: 20px;
					font-size: 2rem;
					color: $white;
					transition: linear 0.1s;
					&:hover{
						color: $monza;
					}
					
				}
				}
				.header-button{
								padding: 15px 30px;
								margin-left: 40px;
								background: $dodgerBlue;
								color: $white;
								transition: linear 0.2s;
								&:hover{
									background: $monza;
								}
								@media screen and (max-width: 950px) {
									&{
										display: none;
									}
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
							.burger{
								display: none;
								color: $silver;
								background: none;
								border: none;
								margin: 0 20px;
								transition: linear 0.2s;
								&:hover{
									color: $dodgerBlue ;
								}

								@media screen and (max-width: 950px) {
									&{
										display: inline-block;
									}
								}
							}
					ul {
						display: flex;
						align-items: center;
						@media screen and (max-width: 950px) {
									&{
										display: none;
									}
								}

						li {
							color: $silver;
							margin-right: 40px;
							transition: linear 0.2s;
							cursor: pointer;

							&:last-child{
								margin: 0;
							}
							&:hover{
								color: $white;
							}
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
