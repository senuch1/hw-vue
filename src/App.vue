<script>
export default {
  data: () => {
    return {
      inputText: "",
      formattedText: "",
    };
  },
  methods: {
    formatText() {
      this.formattedText = this.inputText;
    },
  },
};
</script>

<template>
  <div>
    <p>
      <b><i>{{ formattedText }}</i></b>
    </p>
  </div>
  <textarea v-model="inputText" @input="formatText"></textarea>
</template>
  
<style scoped>
</style>
