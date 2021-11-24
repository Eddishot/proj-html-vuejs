<template>
    <div class="header-container">
      <Navbar></Navbar>

      <div class="row my-2 align-items-center jumbo">
          <div class="col title-jumbo">
              <h1>
                 <strong>Business Planning</strong><br>
                 Digital Technology <br>
                 <strong>modern Solution</strong>

              </h1>
              <p>
                  When, while the lovely valley seems with vapour around <br> mean the meridian sun strikes the upper surface.
              </p>
              <button class="my-button-secondary ">
                  Try it Now
              </button>
              <button class="my-button-primary mx-3">
                  Explore more
              </button>

          </div>
          <div class="col img-jumbo">
              <img class="w-100" src="@/assets/header.png" alt="">
          </div>

      </div>


    </div>
</template>

<script>
import Navbar from "./Navbar.vue"

export default {
name:"Header",
components:{
    Navbar,
}
}
</script>

<style lang="scss">
    .header-container{
        background: linear-gradient(90deg, rgba(1,17,52,1) 29%, rgba(0,32,102,1) 100%);
        color: white;
       
        .jumbo{
            width: 90%;
            margin: auto;

            .title-jumbo{
                p{
                    font-size: 12px;
                }
            }

            .img-jumbo{
                width: 500px;
                margin-bottom: 100px;
            }
        }   

       
    }
</style>