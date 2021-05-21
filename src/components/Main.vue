<template>
<div class="main">
    <div class="jumbotron">

    </div>

    <button class="current">
        CURRENT SERIES
    </button>

    <button class="load">
        LOAD MORE

    </button>

  <div class="containerImgs">
       <PicturesArr 
   v-for="(picture, index) in pictures"
   :key="index"
   :img="picture"
   
   />
  
  </div>
  
</div>
</template>
<script>

import pictures from "@/assets/dc-comics.js"
import PicturesArr from "@/components/PicturesArr.vue"

export default {
    name: 'Main',
    components: {
        PicturesArr
    },
    data(){
        return{
            pictures
        }
    },
    mounted(){
        console.log(pictures);
        
    }
}

</script>
<style lang='scss' scoped>
.main{

    
    text-align: center;
    background-color: black;
    padding-bottom: 130px;
    position: relative;
    
    .jumbotron{
        width: 100%;
        height: 350px;
        background-image: url("../assets/img/jumbotron.jpg");
        background-size: 100%;
        background-repeat: no-repeat;
        padding-bottom: 20px;
    }
   
    .current{
        width: 150px;
        height: 40px;
        color: white;
        background-color: blue;
        font-family: 'Raleway', sans-serif;
        font-weight: 800;
        position: absolute;
        top: 335px;
        left: 100px;
    }
    .load{
        width: 150px;
        height: 40px;
        color: white;
        background-color: blue;
        font-family: 'Raleway', sans-serif;
        font-weight: 800;
        position: absolute;
        left: 660px;
        top: 1050px;

    }
    .containerImgs{
      
        div{
             margin-left: -150px;
             margin-right: -120px;
             padding-top: 50px;
             padding-bottom: 0px;
             img{
                 height: 120px;
             }
        }
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        margin: 0 auto;
        padding: 0 1rem;
        
       

    }
    
}

</style>