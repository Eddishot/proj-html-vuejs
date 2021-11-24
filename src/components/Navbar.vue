<template>
    <div>
        <div class="my-navbar">
          <div class="logo-container">
             <img src="../assets/white-logo-2.png" alt=""> 
          </div>

          <div>
              <ul>
                  <!-- <li>

                      <a href="#">Home</a>
                  </li>
                  <li>
                      <a href="#">Abouts</a>
                  </li>
                  <li>
                      <a href="#">Services</a>
                  </li>
                  <li>
                      <a href="#">Blog</a>
                  </li>
                  <li>
                      <a href="#">Contact</a>
                  </li>
                   <li>
                      <a href="#">Portfolio</a>
                  </li> -->
                  <li v-for="link, i in navbarLinks" :key="i">
                      <a href="#">{{link.title}}</a>
                  </li>
                  <button >Sign in</button>
                  
                  
                </ul>
          </div>
          
          
        </div>

      <div>

      </div>
    </div>
</template>

<script>
export default {
    name:"Navbar",
    data(){
        return{
            navbarLinks:[
                {
                    title:"Home",
                    // href:"#"
                },
                {
                    title:"About",
                    
                },
                {
                    title:"Services",
                
                },
                {
                    title:"Blog",
                    
                },
                {
                    title:"Contact",
                    
                },
                {
                    title:"Portfolio",
                    
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    @import "~bootstrap/scss/bootstrap";

    .logo-container{
        min-width: 200px;
        padding:15px 0px;
    }

    .my-navbar{
        display: flex;
        justify-content: space-around;
        // background-color: blue;
        align-items: center;
        ul{
            margin: 0;
            li{
                display: inline;
                list-style: none;
                text-decoration:none;
                align-items: center;
                padding: 0px 10px;
                

                a{
                    text-decoration:none;
                    color: white;
                     
                    &:hover{
                        color:red;
                        font-weight: bold;
                    }

                }
                
               
            
            }
            button{
                border-radius: 20px;
                 background: linear-gradient(90deg, rgba(2,0,36,1) 10%, rgba(1,43,100,1) 48%, rgba(0,146,255,1) 83%);
                color:white;
                padding: 5px 18px;
                border: none;
            
            
            }
        }

     }
</style>