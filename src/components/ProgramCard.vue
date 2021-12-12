<template>
	<section class="program" >
    <div class="container">

      <div class="card">
          <i  class="card__icon fas fa-stopwatch"></i> 
          <h2 class="card__title">Team training</h2>
          <h3 class="card__subtitle">Find a parthner</h3>
          <p class="card__txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi praesentium soluta, molestiae consectetur</p>
          <a class="card__more" href="">Find a parthner <i class="fas fa-angle-right"></i></a>
      </div>

      <div class="card">
          <i class="card__icon fas fa-dumbbell"></i>
          <h2 class="card__title">Team training</h2>
          <h3 class="card__subtitle">Find a parthner</h3>
          <p class="card__txt">Lorem ipsum dolor sit amet consecteturLorem ipsum dolor sit amet consecteturLorem ipsum dolor sit amet consectetur adipisicing elit. Quasi praesentium soluta, molestiae consectetur</p>
          <a class="card__more" href="">Find a parthner <i class="fas fa-angle-right"></i></a>
      </div>

      <div class="card">
          <i class=" card__icon  fas fa-weight-hanging"></i>
          <h2 class="card__title">Team training</h2>
          <h3 class="card__subtitle">Find a parthner</h3>
          <p class="card__txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi praesentium soluta, molestiae consectetur</p>
          <a class="card__more" href="">Find a parthner <i class="fas fa-angle-right"></i></a>
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
        background-color: black;
        padding: 100px 0;

    >div{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    .card{
      display: flex;
      align-items: center;
      text-align: center;
      flex-direction: column;
      max-width: 400px;
      margin: 10px 10px;
      padding: 70px 40px;
      border: 3px solid $dodgerBlue;
      transition: linear 0.2s;
      &:hover{
        scale: 1.02;
        
      }
      .card__icon{
        color: $white;
        font-size: 4.375rem;
        margin-bottom: 35px;
      }
      .card__title{
        font-size: 1.25rem;
        color: $white;
        margin-bottom: 15px;

      }
      .card__subtitle{
        font-size: 1.25rem;
        color: $yellow;
        margin-bottom: 50px;

      }
      .card__txt{
        color: $silver;
        margin-bottom: 40px;

      }
      .card__more{
        color: $white;
      }
    }
  }
  
</style>
