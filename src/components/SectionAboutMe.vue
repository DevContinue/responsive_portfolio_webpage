<template>
  <section id="about_me_section">
    <img src="@/assets/images/profil.png" alt="" />
    <div class="about_me_container">
      <h2>Über Mich</h2>
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Beatae,
        aliquid! Architecto magni fuga ex dignissimos similique perspiciatis nam
        quisquam eos possimus accusantium quia commodi atque repellat nostrum
        error, consectetur voluptate consequatur ipsum numquam eveniet
        cupiditate. Corrupti ea maxime quas cupiditate aliquid delectus.
        Necessitatibus culpa fuga praesentium, recusandae quia voluptatem atque
        similique ab impedit asperiores quam vel, ducimus neque delectus eum
        blanditiis error omnis labore illo iusto qui dolores? Fuga nesciunt
        obcaecati cum aut hic itaque ea porro inventore modi ipsum dolor
        explicabo veritatis, in iure nam adipisci! Impedit ex cumque magnam
        quidem laboriosam voluptatibus culpa doloribus adipisci, inventore est
        ipsum. Inventore dolorem a possimus aperiam alias vero est fugiat
        voluptatem velit soluta asperiores ratione ipsum vitae minima atque,
        laborum, commodi, autem molestias quisquam ea. Rerum illum eaque
        quibusdam nesciunt? Est.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionAboutMe",
  components: {},

  props: {},
  computed: {},
};
</script>

<style lang="scss">

#about_me_section {
    padding: 100px 0;
    background-color: $second;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 100px;
    flex-wrap: wrap-reverse;

    img {
        width: 400px;
        max-width: 90%;
        border: 8px solid $ciWhite;
    }

}

.about_me_container {
    width: 750px;
    max-width: 90%;

    h2 {
        font-size: 80px;
    }

    p {
        text-align: justify;
        line-height: 175%;
    }
}

@media(max-width: 800px) {
    #about_me_section {
        padding: 50px 0;

        h2 {
            text-align: center;
            font-size: 12vw;
        }
    }
}

</style>
