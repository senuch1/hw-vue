<script>
export default {
  data: () => {
    return {
      product1: {
        src: "/src/assets/img1.jpg",
        alt: "Изображение товара 1",
        title: "Товар 1",
        description: "Описание товара 1",
        price: "100 тенге",
      },
      product2: {
        src: "/src/assets/img2.jpg",
        alt: "Изображение товара 2",
        title: "Товар 2",
        description: "Описание товара 2",
        price: "150 тенге",
      },
    };
  },
};
</script>

<template>
  <div class="product-card">
    <img class="product-img" :src="product1.src" :alt="product1.alt" />
    <h2>{{ product1.title }}</h2>
    <p>{{ product1.description }}</p>
    <p>Цена: {{ product1.price }}</p>
  </div>

  <div class="product-card">
    <img class="product-img" :src="product2.src" :alt="product2.alt" />
    <h2>{{ product2.title }}</h2>
    <p>{{ product2.description }}</p>
    <p>Цена: {{ product2.price }}</p>
  </div>
</template>

<style scoped>
.product-img {
  width: 300px;
  height: 300px;
}
</style>