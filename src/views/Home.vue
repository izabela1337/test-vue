<template>
  <div class="home">
    <b-container>
      <b-row align-v="center">
      <card>..</card>
      <card>..</card>
      <card>..</card>
      </b-row>
    </b-container>
  </div>
</template>

<script>
// @ is an alias to /src
import card from "@/components/card.vue";

export default {
  name: "Home",
  components: {
    "card": card,
  }
};
</script>
