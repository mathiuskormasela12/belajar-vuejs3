<template>
  <h1>Belajar Vue Js</h1>
  <p>Value nya adalah {{ title }}</p>
  <!-- Shorthand -->
  <input type="text" placeholder="Type the movie title" v-model="title" />
  <!-- <input
    type="text"
    placeholder="Type the movie title"
    :value="title"
    @input="title = $event.target.value"
  /> -->
  <!-- Membuat conditional rendering -->
  <p v-if="title === 'naruto'">Naruto Siampudan</p>
  <p v-else-if="title === 'boruto'">Boruto Siakkangan</p>
  <p v-else>404</p>

  <p>Skill saya</p>
  <ol>
    <li v-for="(item, index) in skills" :key="item.id">
      {{ index }} - {{ item.name }}
    </li>
  </ol>
</template>

<script>
/*
    ================= Belajar V-Model, Conditional Rendering & Looping =================

    A. V-Model
       V-Model merupakan berungsi untuk mengubah nilai
       dari sebuah data menggunakan sebuah
       element input HTML.
*/
export default {
  data() {
    return {
      title: "",
      skills: [
        { id: 1, name: "Node Js" },
        { id: 2, name: "Vue Js" },
      ],
    };
  },
};
</script>
