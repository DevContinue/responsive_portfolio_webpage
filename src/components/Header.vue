<template>
  <header>
    <div class="header_text">
      <nav>
        <ul>
          <li><a href="">Über Mich</a></li>
          <li><a href="">Dienstleistungen</a></li>
          <li><a href="">Mehr Informationen</a></li>
        </ul>
      </nav>
      <h1>Dein Name, <br /> <span style="color:royalblue">Webdeveloper</span></h1>
      <p class="subheading">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Non dolor
        recusandae corporis accusamus autem pariatur harum ea et impedit. Neque,
        reiciendis optio. Incidunt perferendis culpa obcaecati ab eos.
      </p>
    </div>
    <div class="circle">
        <img src="@/assets/images/profil.png" alt="">
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  components: {},

  props: {},
  computed: {},
};
</script>

<style lang="scss">

header {
    padding: 50px 25px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 50px;
    flex-wrap: wrap;
}

.header_text {
    width: 850px;
}

.circle {

    height: 300px;
    width: 300px;

    max-width: 80vw;
    max-height: 80vw;

    overflow: hidden;
    border-radius: 50%;
    border: 10px solid royalblue;

    display: flex;
    justify-content: center;
    align-items: center;   
    
    img {
        width: 100%;
    }     

}

nav {
    margin-bottom: 120px;
    position: relative;

    ul {
        list-style: none;
        display: flex;
        gap: 20px;
    }

    a {        
        color: $ciGrey;
        text-decoration: none;    
        position: relative;
        padding: 3px;
    } 

    a:hover {
        color: $ciWhite;
    }
    
    a::after{
        content: "";
        height: 2px;
        width: 0;
        background-color: royalblue;
        position: absolute;
        bottom: 0;
        left: 0;
        transition: 150ms ease-in-out;
    }

    a:hover::after {
        width: 100%;
    }
}

</style>
