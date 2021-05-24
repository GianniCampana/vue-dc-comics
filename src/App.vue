<template>
  <div id="app">
    
    <Header />

    <Main />

    <Footer />

  </div>
</template>

<script>
import Header from "./components/Header"

import Main from "./components/Main"
import Footer from "./components/Footer"

export default {
  name: 'DC',
  components: {
    Header,
    Main,
    Footer

  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  
}


</style>
