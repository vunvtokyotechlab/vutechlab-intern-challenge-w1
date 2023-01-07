<script setup lang="ts">
import ItemCard from "../components/ItemCard.vue";

const itemCardList = [
  {
    icon: "/vectors/vector_1.png",
    title: "4pt grid system",
    content:
      "Base on 4pt grid system. Our UI kit help you create perfect white space",
  },
  {
    icon: "/vectors/vector_2.png",
    title: "Color style",
    content:
      "All color in OpenArt are styled. You can change all design color with one click",
  },
  {
    icon: "/vectors/vector_3.png",
    title: "Free font",
    content:
      "OpenArt use Epilogue font family Available with open licence in gooogle font",
  },
  {
    icon: "/vectors/vector_4.png",
    title: "Darkmode avaiable",
    content:
      "Our UI Kit support darkmode Chage your design to dark mode with one click",
  },
  {
    icon: "/vectors/vector_5.png",
    title: "Easy to customize",
    content: "Create any design with OpenArt UI kits ",
  },
  {
    icon: "/vectors/vector_6.png",
    title: "Variant components",
    content: "All component art variant, easy to design, easy to control",
  },
];
</script>
<template>
  <div class="item-card-list">
    <ItemCard
      v-for="item in itemCardList"
      :icon="item.icon"
      :title="item.title"
      :content="item.content"
    ></ItemCard>
  </div>
</template>
<style scoped>
.item-card-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 80px;
  max-height: 170px;
  box-sizing: border-box;
}
</style>
