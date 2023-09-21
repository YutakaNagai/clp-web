<script setup>
import { ref } from "vue";

defineProps({
  cardInfo: Object,
});
</script>

<template>
  <div class="card" style="width: 38rem">
    <img :src="cardInfo.src" class="card-img-top" :alt="cardInfo.alt" />
    <div class="card-body">
      <h5 class="card-title" v-html="cardInfo.title"></h5>
      <p class="card-text">
        {{ cardInfo.contents }}
      </p>
      <a :href="cardInfo.targetUrl" class="btn btn-primary">詳しくはこちら</a>
    </div>
  </div>
</template>

<style scoped>
.card {
  margin: 0 auto;
}
</style>
