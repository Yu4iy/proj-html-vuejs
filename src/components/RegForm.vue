<template>
	<section>
		<div class="banner box" v-scroll="handleScroll">
			<div class="container">
				<div class="wraper">
					<h2 class="form-banner__subtitle">Join our mailing list today</h2>
					<h3 class="form-banner__title">Insider offers & flash salesin your inbox every week</h3>
					<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="78" height="39" viewBox="0 0 78 39">
					<image id="curvedYline" data-name="curvedYLine" x="3" y="15" width="71" height="12" xlink:href="data:img/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEcAAAAMCAYAAAAwL6CwAAADIElEQVRIiWP8//8/AyHw9Old1h9fF9aLi71QYGL6z/T5M/eH1+/cF+noep4gqJkIcOnC1DR52SvWrKx/WH//Zvn98LHOUT2D7FnUMPvK5e0WokI743h5vwr8+8f47+UriQcc3PGN0tLKvwnpJRg4167u05OVWlnGy307Gln87z+5tdduWm7V1U+fT4njH96r7JGTearEyPAkECb2n0Fm/aMn0vfkldpLKDH78sWZiVrqx72ZmR4FI4t//qq69PGz8C4tbadL+PQzNzQ04JREDphvP5SX37pjN/PFa6OV7Gy/P3Nx3osUEf785+rVl9ziEiYXyHH8w3sVPfIypzz+/eN/ff+hwZrHz5wmf/3Kd4Of74OoIP81i4cPrysJCLrsIsds5ID58FF90a37bn1v3irv5eH585GH604UB8dzvrv3uO+Iiim+xGkIKOVgw1ev7NX79C5tyf+fjv9BNIgPU/f48W3Wp4+KpoDk/nyPX3PpwoxEXObgwg/ulvf8/+l45c/3uDWXL/ZnI6sD8UHiIHmwOhLNBrkH5C6Q+0DuBLkXJnf92iENXP5CxyQHDDUCCF/AUBpA+AKGFP9hDRxiNZIbQMQEDLkBREzAkOJPsgOGnAAiJWBIDSBSAoZY/1IUMKQEEDkBQ2wAkRMwxPib4oDBFUAXz09Jg8k9vEd+wGALILB5UHGQPeQGDKEAYgSV3tISS2pA1TWx9T8u8OTJHVam/9P7pcTPOzAwytz6+Yv1NwvzH2Zmpscaf//J3rh+y3C/jl7BVHLMBoErlyZka6qdd4SZ9+cvy192tt+sDP+fqD17aXjgH2NmoYyMCsHGHTaA3GwBhcPTFzEtzDmZaknSEqfdP39V3U1JwIAAH5/QP15+922PHl1X4uP9LMjC/CiEifHT/5+/Fa9ev2W9UVc/ay65ZoOAmLjF6atXnwkICPzgYWV5qMXC/EHsPwPf24ePtE/IKnYWgewn12xQewfU7gG1f3i5bxu8ecv2A5o050XeunlKjpzkjgs/enST48L5RcGXLm6xpqa58Gx2aasFyHxqmwsKB1B4/P//nwEANOq0NL/yKbEAAAAASUVORK5CYII="/>
					</svg>

					<div class="form-banner__form">
						<input class="btn" type="text">
						<button class="btn" type="submit">Subscribe</button>
					</div>
					<p class="form-banner__txt">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Officiis, beatae! Vero assumenda sapiente non adipisci, error debitis </p>
				</div>
			</div>
		</div>

	</section>
</template>

<script>
export default {
    methods: {
    handleScroll: function (evt, el) {
      if (window.scrollY > 2800) {
        el.setAttribute(
          'style',
          'opacity: 1; transform: translateX(0px)'
        )
      }
      return window.scrollY > 20000
    }
  },		
  props: {
  
  }
}
</script>


<style scoped lang="scss">
	@import "@/styles/variables.scss";

		section{
		background: url('../assets/banner1-2x.jpg');
		background-size: cover;
		width: 100%;
		height: 670px;
		background-position:  right;
		overflow: hidden;

		.banner{
			padding: 20px;
			width: 100%;
			height: 100%;
			position: relative;
			background: linear-gradient(to right, #000000, #000000, #000000ce, #b9b9b900, #ffffff00);
			transform: translateX(50px);
			.container{
				height: 100%;
				display: flex;
				flex-direction: column;
				justify-content: center;
			}
			.wraper{
				max-width: 750px;
				.form-banner__subtitle{
					font-size: 1.375rem;
					color: $monza;
					@media screen and (max-width: 1050px) {
					&{
						font-size: 0.9rem;
					}
				}
				}
				.form-banner__title{
					font-size: 2.8125rem;
					color: $white;
					margin: 30px 0;
					@media screen and (max-width: 1050px) {
					&{
						margin: 15px 0;
						font-size: 2.2rem;
					}
				}
				}
				.form-banner__form{
					display: flex;
					margin: 40px 0 ;
					

					input{
						flex-grow: 1;
						max-width: 580px;
						height: 45px;

					}
					button{
						flex-grow: 1;
						height: 45px;
						max-width: 270px;

						color: $white;
						background-color: $dodgerBlue;
						margin: 0 0 0 35px;
						transition: linear 0.2s;
						&:hover{
							background: $monza;
						}
					}
				}
					.form-banner__txt{
						color: $silver;
					}
			}
			

	

		}
	}
	
</style>
