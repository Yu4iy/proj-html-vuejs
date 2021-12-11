<template>
	<section>
		<div class="video-banner">
			<a class="video__play play" href=""><i class="fas fa-play"></i></a>
			<h2 class="video-banner__title">Crossfit workout of the day</h2>
			<h3 class="video-banner__date">November 15th, 2019</h3>
			<a class="video-banner__link" href="">View all videos</a>
		</div>
	</section>
	foo
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
		background-image: url('../assets/banner14-2x.jpg');
		background-size: cover;
		width: 100%;
		height: 640px;
		background-position: center;
		overflow: hidden;

		.video-banner{
			display: flex;
			align-items: center;
			justify-content: center;
			flex-direction: column;
			width: 100%;
			height: 100%;
			position: relative;
			background: #0818E4;
			background: -webkit-linear-gradient(to bottom right, #082de474 0%, #ce011280 100%);
			background: -moz-linear-gradient(to bottom right, #0817e487 0%, #ce011272 100%);
			background: linear-gradient(to bottom right, #0817e480 0%, #ce011278 100%);
			.video__play{
				width: 100px;
				height: 100px;
				font-size: 20px;
				right: 50%;
				transform: translatey(-50%);
			}
			.video-banner__title{
				font-size: 2.5rem;
				color: $white;
			}
			.video-banner__date{
				font-size: 1.875rem;
				color: $yellow;
				margin: 40px 0 0 0;
			}
			.video-banner__link{
				margin: 30px 0 0 0;
				color: $white;
			}

		}
	}
</style>
