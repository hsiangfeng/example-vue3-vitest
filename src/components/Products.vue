<script setup>
import { onMounted } from 'vue';

const props = defineProps({
  products: {
    type: Array,
    required: true
  }
});

const showAlert = (str) => {
  window.alert(str);
}
</script>

<template>
  <ul>
    <li v-for="item in products">{{ item.title }}</li>
  </ul>
  <button class="btn btn-alert" @click="showAlert('哈囉')">點我</button>
</template>

<style lang="scss" scoped>
</style>