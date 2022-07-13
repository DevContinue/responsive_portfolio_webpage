<template>
  <section id="services_section">
    <h2>Dienst&shyleistungen</h2>
    <div class="flex_container">
      <div class="card" v-for="i in 3" :key="i">
        <h3>Beratung</h3>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nobis
          voluptatibus iste similique tempore laboriosam accusamus consequuntur
          saepe in perspiciatis, vero libero pariatur aliquam corrupti sunt!
          Maiores natus quia cum nobis?
        </p>
        <a href="">Buchen</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionServices",
  components: {},

  props: {},
  computed: {},
};
</script>

<style lang="scss">

#services_section {
    padding: 70px 0;
    background-color: $prime;

    h2 {
        font-size: clamp(80px, 12vw, 50px);
        text-align: center;
    }
}

.flex_container {
    margin-top: 50px;
    display: flex;
    gap: 40px;
    justify-content: center;
    flex-wrap: wrap;

    .card {
        width: 350px;
        max-width: 90%;
        background-color: $second;
        border-radius: 100px;
        padding: 60px 20px;

        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 20px;

        * {
            text-align: center;
        }

        a {
            background-color: royalblue;
            width: min-content;
            padding: 15px 40px;
            border-radius: 50px;
            margin: 0 auto;
            text-decoration: none;
            color: $ciWhite;
            border: 4px solid royalblue;
            transition: 150ms ease-in-out;
        }

        a:hover {
            background-color: transparent;
        }
    }
}

/* @media(max-width: 500px) {
    #services_section h2 {
        font-size: 12vw;
    }    
} */

</style>
