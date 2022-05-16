<template>
  <div>
    <h1>Lifecycle</h1>
  </div>
</template>

<script>
export default {
  // dijalankna ketika component sblm di buat (blm di tempel)
  beforeCreate() {
    console.log("beforeCreate");
  },

  // di jalankan ketika component sudah di buat (blm di tempel)
  created() {
    console.log("created");
  },

  // dijalankan sebelm component di tempel (setelah component di buat)
  beforeMount() {
    console.log("beforeMount");
  },

  // dijalankan sesudah component di tempel (setelah component di buat)
  mounted() {
    console.log("mounted");
  },

  // di jalankan sebelum ketika ada perubahan data dan props
  beforeUpdate() {
    console.log("beforeUpdate");
  },

  // di jalankan ketika ada perubahan data dan props
  updated() {
    console.log("updated");
  },

  //  dijakankan sebelum component di hapus
  beforeUnmount() {
    console.log("beforeUnmount");
  },

  // di jalankan ketika component sudah di hapus
  unmounted() {
    console.log("unmounted");
  },
};
</script>
