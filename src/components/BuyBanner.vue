<template>
	<section>
		<div class="buy-banner">
			<div class="wraper">
				<h2 class="buy-banner__title" >"I've failed over and over again in my life. And that is why i sycceed."</h2>
				<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="78" height="39" viewBox="0 0 78 39">
				<image id="curvedYline" data-name="Слой 1" x="3" y="15" width="71" height="12" xlink:href="data:img/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEcAAAAMCAYAAAAwL6CwAAADIElEQVRIiWP8//8/AyHw9Old1h9fF9aLi71QYGL6z/T5M/eH1+/cF+noep4gqJkIcOnC1DR52SvWrKx/WH//Zvn98LHOUT2D7FnUMPvK5e0WokI743h5vwr8+8f47+UriQcc3PGN0tLKvwnpJRg4167u05OVWlnGy307Gln87z+5tdduWm7V1U+fT4njH96r7JGTearEyPAkECb2n0Fm/aMn0vfkldpLKDH78sWZiVrqx72ZmR4FI4t//qq69PGz8C4tbadL+PQzNzQ04JREDphvP5SX37pjN/PFa6OV7Gy/P3Nx3osUEf785+rVl9ziEiYXyHH8w3sVPfIypzz+/eN/ff+hwZrHz5wmf/3Kd4Of74OoIP81i4cPrysJCLrsIsds5ID58FF90a37bn1v3irv5eH585GH604UB8dzvrv3uO+Iiim+xGkIKOVgw1ev7NX79C5tyf+fjv9BNIgPU/f48W3Wp4+KpoDk/nyPX3PpwoxEXObgwg/ulvf8/+l45c/3uDWXL/ZnI6sD8UHiIHmwOhLNBrkH5C6Q+0DuBLkXJnf92iENXP5CxyQHDDUCCF/AUBpA+AKGFP9hDRxiNZIbQMQEDLkBREzAkOJPsgOGnAAiJWBIDSBSAoZY/1IUMKQEEDkBQ2wAkRMwxPib4oDBFUAXz09Jg8k9vEd+wGALILB5UHGQPeQGDKEAYgSV3tISS2pA1TWx9T8u8OTJHVam/9P7pcTPOzAwytz6+Yv1NwvzH2Zmpscaf//J3rh+y3C/jl7BVHLMBoErlyZka6qdd4SZ9+cvy192tt+sDP+fqD17aXjgH2NmoYyMCsHGHTaA3GwBhcPTFzEtzDmZaknSEqfdP39V3U1JwIAAH5/QP15+922PHl1X4uP9LMjC/CiEifHT/5+/Fa9ev2W9UVc/ay65ZoOAmLjF6atXnwkICPzgYWV5qMXC/EHsPwPf24ePtE/IKnYWgewn12xQewfU7gG1f3i5bxu8ecv2A5o050XeunlKjpzkjgs/enST48L5RcGXLm6xpqa58Gx2aasFyHxqmwsKB1B4/P//nwEANOq0NL/yKbEAAAAASUVORK5CYII="/>
				</svg>

				<p class="buy-banner__txt"> Quibusdam dignissimos dolores architecto pariatur quia consectetur, nobis voluptatibus quis ex numquam molestiae dolorum laborum aperiam obcaecati harum dolor dolore nihil delectus.</p>
				<button class="btn buy-banner-btn">Buy Avada Today <i class="fas fa-angle-right"></i></button>
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
		background-image: url('../assets/banner2-2x.jpg');
		background-size: cover;
		width: 100%;
		height: 640px;
		background-position: center;
		overflow: hidden;

		.buy-banner{
			display: flex;
			align-items: center;
			justify-content: center;
			flex-direction: column;
			width: 100%;
			height: 100%;
			position: relative;
			background: #000000;
			background: -webkit-linear-gradient(to top, #000000 2%, #ffffff00 100%);
			background: -moz-linear-gradient(to top, #000000 2%, #ffffff00 100%);
			background: linear-gradient(to top, #000000 2%, #ffffff00 100%);
				.wraper{
					text-align: center;
					max-width: 780px;
					.buy-banner__title{
						font-size: 2.5rem;
						color: $white;
						margin-bottom: 20px ;
					}
					.buy-banner__txt{
						color: $white;
						margin: 30px 0;


						
					}

					.buy-banner-btn{
						padding: 20px 40px;
						background: $dodgerBlue;
						color: $white;
						transition: linear 0.2s;
						cursor: pointer;
						&:hover{
							background: $monza;
							
						}

					}
					
				
			}

		}
	}	

</style>
