<template>
<div>
   <div class="my-container">
    <div class="row row-cols-2 my-sub-container">
      <div class="row">
        <h3>
         <strong>We Offer Awesome Services</strong> 
        </h3>
        <p>
          When, while lovely valley teems with vapour around meand meridian sun strikes upper surface.
        </p>
      </div>
      <div class="row">
        <form action="">
          <input type="text" placeholder="Enter Your Email Adress">
          <button class="my-button-primary">Subsbribe</button>
        </form>
        
      </div>
    </div>
   
    <div class="row row-cols-4 ">
      <div class="col">
        <img class="logo-img" src="@/assets/white-logo-2.png" alt="">
        <p>
           When, while lovely valley teems with vapour around meand meridian sun strikes upper surface.
        </p> 
      </div>
      <div class="col">
        <ul>
          <li><h6><strong>Quick Links</strong></h6></li>
          <li>Services</li>
          <li>Contact</li>
          <li>Blog</li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <li><h6><strong>Resources</strong></h6></li>
          <li>Art Design</li>
          <li>Computer</li>
          <li>It News</li>
          <li>Networking</li>
          <li>Web Security</li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <li><h6><strong>Contact US</strong></h6></li>
          <li>
            <strong>Address:</strong>Patricia C.Amedee,4401 Waldeck Street Grapevine Nashville,Tx 76051
          </li>
          <li> <strong>Phone:</strong>+99(0)1010000888</li>
          <li> <strong>Email:</strong>info@yourdomain.com</li>
        </ul>
      </div>
      <div class="col">
        <hr>
        <p>2020 Phlox. All Rights Reserved</p>
      </div>
      
      
    </div>
  </div>
</div>
 
</template>

      

<script>
export default {
  name:"Footer",

  data(){
    return{
      quickLinks:["Quick Links", "Services","Contact","Blog"],
      resources:["Resources","Art Design", "Computer", "It  News","Networking","Web Security"],
      
      
    }
  }
}
</script>

<style lang="scss">
.my-sub-container{
  
  width: 1200px;
  background: linear-gradient(90deg, rgba(140,10,0,1) 29%, rgba(249,30,2,1) 100%);
  border-radius: 12px;
  padding: 20px;
  margin: auto;
  align-items: center;
  justify-content: space-between;
  color: white;
   
    form {
  display:flex;
  flex-direction:row;
  padding:5px 6px 5px 40px;
  border-radius: 30px;
  background-color: white;
  border:1px solid grey;
 
  
  input{
    border:none;
     color: lightgrey;
    flex-grow:2;
    // width: 300px;

    &:focus{
      outline: none;
    }

      
  }
}
.logo-img{
  color: black;
  min-width: 100px;
  background-color: black;
}
  
}
</style>