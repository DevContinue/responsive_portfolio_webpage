<template>
  
  <Header />
  
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header,
  },

  props: {
    
  },
  computed: {
    
  },
}
</script>
<style lang='scss'>

html,
body {
  width: 100%;
  height: 100%;
  background-color: $second;
  color: $ciWhite;
  font-size: 20px;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

h1{
  font-size: 50px;
  line-height: 115%;
}

.subheading {
  margin-top: 25px;
  color: $ciGrey
}

@media (max-width: 800px) {
  h1 {
    font-size: 12vw;
    text-align: center;
  }
  .subheading {
    text-align: center;
  }
}

</style>