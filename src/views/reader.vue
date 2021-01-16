<template>
  <div class="container-fluid">
    <readertop></readertop>
    <div class="container">
      <button class="buttonprev" @click="$refs.slider.prev()">prev</button>
      <button class="buttonnex" @click="$refs.slider.next()">next</button>
      <ReaderSlider ref="slider" :options="options" :items="items">
        <template v-slot:item="{ item, index, active }">
          <ReaderItem :index="index" :active="active">
            <img @click="$refs.slider.next()" :src="item.src" />
            <p>Strona {{ index + 1 }}</p>
            <template v-slot:loading>
              <p>
                Ładowanie... albo koniec. Albo nawet nie wiem. Czasami się
                psuje.
              </p>
            </template>
          </ReaderItem>
        </template>
        <template v-slot:pagination="{ item, current, total }">
          <ReaderPagination :current="current" :total="total">
            <div>{{ current + "/" + total }}</div>
          </ReaderPagination>
        </template>
      </ReaderSlider>
    </div>
    <readerbot></readerbot>
  </div>
</template>

<script>
import readertop from "@/components/readertop.vue";
import readerbot from "@/components/readerbot.vue";

export default {
  name: "Reader",
  components: {
    readertop: readertop,
    readerbot: readerbot
  },
  data() {
    const items = [];
    for (let i = 1; i <= 6; i++) {
      items.push({ src: `/manga/3/` + (i < 10 ? `00` : `0`) + `${i}.jpg` });
    }
    return {
      items,
      options: {
        virtual: true,
        pagination: true,
        direction: "vertical",
        margin: "0px",
        width: "auto",
        height: "800px",
        inertia: true,
        loading: true,
        batch: 5,
        speedLimit: { down: 0.2, up: 8 }
      }
    };
  }
};
</script>

<style lang="scss" scoped>
img {
  max-height: 100%;
  max-width: 100%;
  // height: 70vh;
}
.sc-reader-item-vertical img {
  display: initial;
  height: 80vh;
  width: auto;
}
.sc-reader-item-list {
  background-color: rgb(17, 17, 17);
}
.buttonprev {
  position: fixed;
  left: 10px;
  top: 50%;
}
.buttonnex {
  position: fixed;
  right: 10px;
  top: 50%;
}
</style>
