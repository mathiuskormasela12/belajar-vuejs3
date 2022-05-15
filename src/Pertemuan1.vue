<template>
  <div>
    <h1>Belajar Vue Js</h1>
    <!-- Mencetak data -->
    <p :title="nama">Hi my name is {{ nama }}</p>
    <p>Di Klik {{ count }}</p>
    <!-- Memanggil method -->
    <button type="button" @click="increment">Count</button>
    <button type="button" @click="count--">Decrement</button>
  </div>
</template>

<script>
export default {
  /*
    ============ Belajar Declarative Rendering & Methods ============
    
    A. Data
       Data merupakan sebuah variable seperti 
       state dalam React Js. Ketika value data nya
       berubah, otomatis componentnya akan
       di render ulang.

    B. Declarative Rendering
       Declarative rendering merupakan cara kita
       untuk mencetak nilai dari data.

    C. Methods
       Method merupakan kumpulan function atau event
       yang dapat di panggil.
  */
  data() {
    return {
      nama: "Mathius",
      count: 0,
    };
  },

  methods: {
    increment() {
      this.count += 1;
    },
  },
};
</script>
