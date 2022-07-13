<template>
  <header>
    <div class="header_text">
      <nav>        
        <input type="checkbox" id="toggle_button">
            <label for="toggle_button">
                <span class="material-symbols-rounded"> menu </span>
            </label>
        <ul>
          <li><a href="#about_me_section">Über Mich</a></li>
          <li><a href="#services_section">Dienstleistungen</a></li>
          <li><a href="">Mehr Informationen</a></li>
        </ul>
      </nav>
      <h1>
        Dein Name, <br />
        <span style="color: royalblue">Webdeveloper</span>
      </h1>
      <p class="subheading">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Non dolor
        recusandae corporis accusamus autem pariatur harum ea et impedit. Neque,
        reiciendis optio. Incidunt perferendis culpa obcaecati ab eos.
      </p>
    </div>
    <div class="circle">
      <img src="@/assets/images/profil.png" alt="" />
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
  padding: 100px 25px;
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

  a::after {
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

#toggle_button {
    display: none;
}

label[for="toggle_button"]{
    display: none;
}
    
label[for="toggle_button"] span{
    font-size: 40px;
}

@media (max-width: 800px) {
    nav {
        position: absolute;
        top: 0;
        left: 0;
        background-color: #3b494d;
        padding: 15px;
        border-radius: 0 0 25px 0;

        ul {
            display: none;
            flex-direction: column;
        }
    }

    #toggle_button:checked ~ ul {
        display: flex;
    }  
    
    label[for="toggle_button"] {
        display: block;
    }

}


</style>
