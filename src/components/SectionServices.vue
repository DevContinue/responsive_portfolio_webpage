<template>
  <section id="services_section">
    <h2>Dienstleistungen</h2>
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

<style lang="scss"></style>
