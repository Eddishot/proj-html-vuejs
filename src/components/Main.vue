<template>
    <div>
        <div class="my-section">
            <div>
                <p style="color:red;">Our Services </p>
                <h1>
                    <strong>What</strong>We do
                </h1>
                <p>When,while the lovely valley teems with vapour around meand the</p>
            </div>
            <div class="row my-card">
                <div class="col" v-for="dati,i in miniCard" :key="i">
                    <img :src="dati.img" alt="logo">
                    <h3><strong>{{dati.title}}</strong></h3>
                    <p>{{dati.paragraph}}</p>
                </div>
           
            </div>
                <div class="my-button">
                <button class="my-button-secondary">View All Services</button>
            </div> 
        </div>
      
    </div>
</template>

<script>
export default {
    name:"Main",
    data(){
        return{
           
            miniCard:[

                {
                  img: require('../assets/Group-247.png'),
                title:"Data Analysis",
                paragraph:"When,while the lovely valley teems with vapour around meand the meridian sun strikes the upper",  
                },
                 {
                  img:require("../assets/Group-567.png"),
                title:"Seo Optimization",
                paragraph:"When,while the lovely valley teems with vapour around meand the meridian sun strikes the upper",  
                },
                 {
                  img:require("../assets/Group-538.png"),
                title:"Security Data",
                paragraph:"When,while the lovely valley teems with vapour around meand the meridian sun strikes the upper",  
                },
                 {
                  img:require("../assets/Group-566.png"),
                title:"Branding Strategy",
                paragraph:"When,while the lovely valley teems with vapour around meand the meridian sun strikes the upper",  
                },
                

            ],
              
            

        }
        
    }

}
</script>

<style lang="scss">
    .my-section{
        margin:auto;
        width: 80%;
        text-align: center;
        padding:40px 0px;
        gap: 50px;

        .my-card{
            margin: 120px 0px;
            gap: 50px;

            img{
                // width:130;
                height: 180px;
                padding-bottom: 50px;
            }
            
            h3{
                padding-bottom: 20px;
            }
            p{
                font-size: 14px;
                color: rgb(75, 75, 75);
            }

                
        }
        .my-button{
            margin-bottom:50px;

            
        }
    }
</style>