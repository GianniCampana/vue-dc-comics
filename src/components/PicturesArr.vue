<template>
  <div>
      <img :src="img.thumb" :alt="img.series">
      <h2>{{img.series}}</h2>
  </div>
</template>

<script>
export default {
    name: 'Pictures',
    props:{
      img: Object
    }

}
</script>

<style lang="scss" scoped>

div{

  img{
    height: 250px;
    margin: 0%;
  }
  h2{
    color: white;
    font-size: 12px;
    font-family: 'Raleway', sans-serif;
  }
  flex-basis: calc(100% / 3);
}

</style>