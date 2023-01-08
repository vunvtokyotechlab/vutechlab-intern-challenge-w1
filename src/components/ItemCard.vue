<script setup lang="ts">
interface IProps {
  icon: string;
  title: string;
  content: string;
}

defineProps<IProps>();
</script>
<template>
  <div class="item-card w-reponsive">
    <img :src="icon" />
    <p class="item-card__title">{{ title }}</p>
    <p class="item-card__content">
      {{ content }}
    </p>
  </div>
</template>
<style scoped>
.item-card {
  font-style: normal;
  font-weight: 400;
  color: #000;
  background-color: #ffffff;
  margin-top: 30px;
  border-radius: 16px;
  padding: 18px;
  overflow: auto;
}
.item-card:hover {
  border: 2px solid rgb(75, 106, 168);
  cursor: pointer;
}
.item-card__title {
  font-size: 1.5rem;
  line-height: 25px;
  color: #333333;
}
.item-card__content {
  font-size: 1rem;
  line-height: 21px;
  color: #555;
}
</style>
