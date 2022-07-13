<template>
  
  <Header />
  <SectionAboutMe />
  
</template>

<script>
import Header from './components/Header.vue'
import SectionAboutMe from './components/SectionAboutMe.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionAboutMe,
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
  background-color: $prime;
  color: $ciWhite;
  font-size: 20px;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

h1{
  font-size: 100px;
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