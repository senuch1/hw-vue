<script>
export default {
  data: () => {
    return {
      colors: [
        { name: "Красный", code: "#FF0000" },
        { name: "Зеленый", code: "#00FF00" },
        { name: "Синий", code: "#0000FF" },
        { name: "Желтый", code: "#FFFF00" },
        { name: "Фиолетовый", code: "#800080" },
        { name: "Оранжевый", code: "#FFA500" },
        { name: "Розовый", code: "#FFC0CB" },
      ],
    };
  },
};
</script>

<template>
  <div class="color-card" v-for="(color, index) in colors" :key="index">
    <div class="color-box" :style="{backgroundColor: color.code }"></div>
    <p>{{ color.name }}</p>
    <p>{{ color.code }}</p>
  </div>
</template>
  
<style scoped>
.color-card {
  display: inline-block;
  width: 150px;
  margin: 10px;
  padding: 10px;
  text-align: center;
  border: 1px solid #ccc;
}
</style>
