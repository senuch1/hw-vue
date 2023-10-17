<script>
export default {
  data: () => {
    return {
      name: '',
      age: []
    };
  },
};
</script>

<template>
  <form>
      <label for="name">Имя: </label>
      <input type="text" id="name" v-model="name">
      <br>
      <label for="age">Возраст: </label>
      <input type="number" id="age" v-model="age">
    </form>

    <div v-if="age < 0">
      <p>Это как</p>
    </div>
    <div v-else-if="age < 18">
      <p>Привет, {{ name }} пока туда сюда двигаемся молодые</p>
    </div>
    <div v-else-if="age <= 100">
      <p>Привет, {{ name }} вы взрослый</p>
    </div>
    <div v-else>
      <p>Агай вам хорошо??</p>
    </div>
</template>
  
<style scoped>
</style>
