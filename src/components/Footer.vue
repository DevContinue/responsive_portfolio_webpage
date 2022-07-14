<template>
  <footer id="more_information">
    <h2>Mehr Informationen</h2>
    <div class="grid_container">
      <div id="item1" class="grid_item">
        <img src="@/components/icons/instagram-svgrepo-com.svg" alt="" />
        <div>
          <h3>Instagram</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Error velit
            nihil adipisci voluptatem in repudiandae!
          </p>
        </div>
      </div>
      <div id="item2" class="grid_item">
        <img src="@/components/icons/telegram-svgrepo-com.svg" alt="" />
        <h3>Telegram</h3>
      </div>
      <div id="item3" class="grid_item">
        <h3>Kontakt</h3>
        <p>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis cum
          nostrum possimus veritatis delectus minima non. Voluptatibus magni,
          sequi obcaecati molestias facilis perferendis repellat ipsa?
        </p>
      </div>
      <div id="item4" class="grid_item">
        <img src="@/components/icons/twitter-svgrepo-com.svg" alt="" />
        <h3>Twitter</h3>
      </div>
      <div id="item5" class="grid_item">
        <img src="@/components/icons/youtube-svgrepo-com.svg" alt="" />
        <div>
          <h3>Youtube</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Error velit
            nihil adipisci voluptatem in repudiandae!
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  components: {},

  props: {},
  computed: {},
};
</script>

<style lang="scss">
footer {
  padding: 70px 0;
  background-color: $second;

  h2 {
    font-size: 50px;
    text-align: center;
  }
}

.grid_container {
  margin: 60px auto;
  width: 1500px;
  max-width: 90%;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 300px 300px;
  gap: 15px;
  grid-template-areas:
    "item1 item1 item2 item3 "
    "item4 item5 item5 item3";

  .grid_item {
    background-color: #3f5663;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 50px;
    gap: 50px;

    img {
      height: 150px;
      width: 150px;
    }
  }

  #item1 {
    grid-area: item1;
  }

  #item2 {
    grid-area: item2;
    flex-direction: column;
    gap: 10px;
  }

  #item3 {
    grid-area: item3;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 10px;
  }

  #item4 {
    grid-area: item4;
    flex-direction: column;
    gap: 10px;
  }

  #item5 {
    grid-area: item5;
  }
}

@media(max-width: 1300px) {
    .grid_container {
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 300px 300px 300px;
        grid-template-areas:
        "item1 item1 item2"
        "item4 item5 item5"
        "item3 item3 item3";
    }
}

@media(max-width: 900px) {
    .grid_container {
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto auto auto auto;
        grid-template-areas:
        "item1 item1"
        "item5 item5"
        "item2 item4"
        "item3 item3";
    }
}

@media(max-width: 650px) {
    footer h2{
        font-size: 9vw;
    }

    .grid_item {
        padding:20px;

        img {
            height: 100px;
            width: 100px;
        }

        h3 {
            font-size: 24px;
        }
    }
}

</style>
