<template>
  <div>
    <h1>V-Once</h1>
    <!-- Hanya akan di render sekalih -->
    <!-- <p v-once>{{ value }}</p> -->
    <!-- Merender data sebagai html -->
    <p v-html="value"></p>
    <input type="text" v-model="value" />
    <p>{{ cetak }}</p>
    <p>Ini bre {{ print }}</p>
    <button @click="print = 'Test'">Test</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      value: "lama",
    };
  },

  computed: {
    cetak() {
      return "Hello WOrld";
    },
    print: {
      get() {
        return this.value;
      },
      set(val) {
        this.value = val.toUpperCase();
      },
    },
  },
};
</script>
