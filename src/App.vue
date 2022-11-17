<template>
  <h1 :class="{ 'title' : false, 'title-home' : isHome }">
    Curso Vue 3
  </h1>

  <p :class="pClass">
    Id in occaecat proident consequat reprehenderit commodo officia esse adipisicing aliquip proident incididunt.
  </p>

  <div v-for="(obj, index) in todos" :key="obj.id" class="todos-item">
    <img v-if="obj.imgSrc" :src="obj.imgSrc">
    {{ index }} {{ obj.title }}
  </div>
</template>



<script>
  export default {
    name: 'App' ,
    data() {
      return {
        classVar: "title",
        pClass: ['text', 'text-home'],
        isHome: true,
        todos: [
          {
            "userId": 1,
            "id": 1,
            "title": "delectus aut autem",
            "completed": false,
            "imgSrc": "https://via.placeholder.com/150",
          },
          {
            "userId": 1,
            "id": 2,
            "title": "quis ut nam facilis et officia qui",
            "completed": false,
            "imgSrc": "https://via.placeholder.com/150",
          },
          {
            "userId": 1,
            "id": 3,
            "title": "fugiat veniam minus",
            "completed": false
          },
          {
            "userId": 1,
            "id": 4,
            "title": "et porro tempora",
            "completed": true
          },
          {
            "userId": 1,
            "id": 5,
            "title": "laboriosam mollitia et enim quasi adipisci quia provident illum",
            "completed": false
          }
        ]
      }
    }
  }
</script>



<style>
  .text {
    color: blue;
  }

  .text-home {
    font-size: 40px;
    color: blue;
  }

  .title-home {
    font-size: 100px;
    color: black;
    background-color: aqua;
  }

  .title {
    font-size: 50px;
    color: black;
    background-color: aqua;
  }

  .todos-item {
    background-color: blueviolet;
    margin: 0 0 5px 0;
    padding: 3px 6px;
    color: white;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin: 60px;
  }
</style>
