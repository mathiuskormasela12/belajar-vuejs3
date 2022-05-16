<template>
  <div>
    <h1>Belajar Looping Dengan Component</h1>
    <my-title v-for="num in numbers" :key="num" :title="num" />
  </div>
</template>

<script>
import MyTitle from "./components/MyTitle.vue";

export default {
  components: {
    MyTitle,
  },
  data() {
    return {
      numbers: [1, 2, 3],
    };
  },
};
</script>
