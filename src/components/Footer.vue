<template>
    <div class="footer">

      


     <div class="liste">
      <ul>
         <li class="first-element-list">DC COMICS</li>
         <li>Characters</li>
         <li>Comics</li>
         <li>Movies</li>
         <li>TV</li>
         <li>Games</li>
         <li>Video</li>
         <li>News</li>
      </ul>

      <ul>
         <li class="first-element-list">DC</li>
         <li>Terms Of Use</li>
         <li>Privacy policy(New)</li>
         <li>Ad Choices</li>
         <li>Advertising</li>
         <li>Jobs</li>
         <li>Subscriptions</li>
         <li>Talent Workshops</li>
         <li>CPSC Certificates</li>
         <li>Ratings</li>
         <li>Shop Help</li>
         <li>Contact us</li>
      </ul>

      <ul>
          <li class="first-element-list">SITES</li>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>

      </ul>

      <ul class="shop">
         <li class="first-element-list">SHOP</li>
         <li>Shop DC</li>
         <li>Shop DC Collectibles</li>
      </ul>
      
    </div>
        
    
    <div class="last-footer">

        <button>
            <p>SIGN-UP NOW!</p>
        </button>

        <div class="contacts">
            <h1>FOLLOW US</h1>
            <img src="../assets/img/footer-facebook.png" alt="">
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
        </div>

    </div>

    </div>
</template>

<script>
export default {
    name: 'Footer',
    components: {
     
    }
    
}
</script>

<style lang='scss' scoped>
.footer{
    width: 100%;
    height: calc(100vh - 200px);
    background-image: url("../assets/img/dc-logo-bg.png"), url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size:30%, cover;
    background-position: 800px, center;
    padding-top: calc((100vh - 200px) - 100px);
    img{
        margin-left: 55%;
        margin-top: 50px;
        width: 30%;
        
    }
    .liste{
        position: relative;
        padding-top: 150px;
        width: 30%;
        height: calc((100vh - 200px) - 100px) ;
        margin-top: -455px;
        margin-left: 150px;
        font-family: 'Raleway', sans-serif;
        font-size: 10px;
        color: white;
        .shop{
            position: absolute;
            top: 300px;
        }
        
        ul{
            float: left;
            margin-left: 60px;
            .first-element-list{
                font-family: 'Raleway', sans-serif;
                font-weight: 500;
                font-size: 15px;
                margin-bottom: 7px;
                color: white;

            }
            li{
                list-style: none;
                color: rgb(199, 199, 199);
                margin-top: 5px;
                cursor: pointer;
            }
        }
        
    }
    
    .last-footer{
        height: 100px;
        width: 100%;
        background-color: rgb(54, 54, 54);
        display: flex;
        align-items: center;

        button{
            margin-left: 210px;
            padding: 10px;
            background-color: rgb(54, 54, 54);
            border: solid 3px rgb(67, 67, 255);
            cursor: pointer;

            p{
                font-family: 'Raleway', sans-serif;
                font-weight: 500;
                font-size: 15px;
                color: white;
            }
            
        }

        .contacts{
            display: flex;
            align-items: center;
            height: 100px;
            width: 30%;
            margin-left: 500px;
            h1{
                color: blue;
                font-family: 'Raleway', sans-serif;
                font-weight: 600;
                font-size: 20px;
            }
            img{
                width: 40px;
                margin-left: 20px;
                margin-bottom: 50px;
                cursor: pointer;
            }
            
        }
     
       
    }
}

</style>