<template>
	<section>
		<div class="container">
			<div class="title">
				<h2 class="title__txt">Latest Articles</h2>
				<button class="title__show-btn">Read all articles <i class="fas fa-angle-right"></i></button>
			</div>
		</div>
		<div class="cards">

			<div class="container">
				<div class="card box" v-scroll="handleScroll" v-for="(elem,index) in posts" :key= 'index'>
						<div class="card__img">
							<img :src="require(`../assets/${elem.img}.jpg`)" alt="card" />
						</div>
						
						<h3 class="card__title">{{elem.title}}</h3>
						<div class="card__date">{{elem.postedBy}} | {{elem.date}} | {{elem.article}}</div>
				</div>


			</div>
	</div>
	</section>		
</template>

<script>
export default {
    methods: {
    handleScroll: function (evt, el) {
      if (window.scrollY > 3700) {
        el.setAttribute(
          'style',
          'opacity: 1; transform: translateX(0px)'
        )
      }
      return window.scrollY > 20000
    }
  },
  props: {
	posts:Array
  }
}
</script>


<style scoped lang="scss">
@import "@/styles/variables.scss";

.cards{
        padding: 0 0 130px 0;
		@media screen and (max-width: 1260px) {
			&{
				padding: 0 0 30px 0;

					}
				}

    >div{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    .card{
		transform: translateX(50px);
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
				position: relative;
				
					&::after{
						content: ' ';
						background: rgb(0,0,0);
						background: linear-gradient(180deg, rgba(0, 0, 0, 0) 0%, rgba(84, 101, 199, 0.671) 100%);
						width: 100%;
						height: 100%;
						position: absolute;
						border-radius:  5px;
						opacity: 0;
						transition: linear 0.2s;
						
					}
						&:hover::after{
							opacity: 1;
							
						}
				
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
			padding: 10px;

			.title__show-btn{
					border: none;
					background: none;
					font-weight: 600;
				}
	}

</style>
