<template>

  <!--OBSERVADORES (WATCH)-->
  <div>
    <!--
    <div>

      <input v-model="name" type="text"> <br>

      {{ name }}

      <br><br><br>

      <input v-model="user.firstName" type="text"> <br> <br>
      <input v-model="user.lastName" type="text"> <br>

      {{ user.firstName }} {{ user.lastName }}

      <br><br><br>

      <select v-model="pageCount">
        <option value="5">5</option>
        <option value="10">10</option>
        <option value="15">15</option>
      </select> <br>

      {{ pageCount }}

    </div>
    -->
  </div>
  <!--FIM OBSERVADORES (WATCH)-->



  

  <!--PROPRIEDADES COMPUTADAS (FILTRO)-->
  <div>
    <!--
    <div>
      {{ fullName }}
    </div> 
  
    <br>
  
    <h2>Todos em aberto</h2>
    <div v-for="a in unComletedTodos" :key="a.id">
      {{ a.title }} <span>{{ a.completed }}</span>
    </div>
  
    <h2>Todos completas</h2>
    <div v-for="a in comletedTodos" :key="a.id">
      {{ a.title }} <span>{{ a.completed }}</span>
    </div>
  
    <br><br>
  
    <h2>Todos</h2>
    <div v-for="a in todos" :key="a.id">
      <input v-model="a.completed" type="checkbox"> 
      {{ a.title }}
    </div>
    -->
  </div>
  <!--FIM PROPRIEDADES COMPUTADAS-->





  <!--EVENTOS-->
  <div>
    <!--
    <div>
      <div>
        <button @click="onClick">CLIQUE</button>
      </div>
    
      <div @mouseover="onMouseOver" @mouseout="onMouseOut">
        Mouse over
      </div>
    
      <br><br>
    
      <form @submit.prevent="onSubmit" action="https://google.com">
    
        <input type="text" @keyup.enter="onKeyUp">
    
        <button type="submit">Enviar</button>
    
      </form>
    </div>
    -->
  </div>
  <!--FIM EVENTOS-->





  <!--LIGAÇÃO DE DADOS (v-model)-->
  <div>
    <!--
    <div>
      Two-Way data binding <br>
      One-Way data biding <br>
      v-model -> formulários
    </div>

    <br><br>

    <div>
      <label>Name</label> <br>
      <input type="text" v-model="name">

      <br> <br>

      {{ name }}

      <br><br>
    </div>

    <div>
      <label>Sports</label> <br>
      <select v-model="sports">
        <option value="futebol">Futebol</option>
        <option value="handball">Handball</option>
        <option value="volei">Volei</option>
        <option value="basquete">Basquete</option>
      </select>

      <br><br>

      {{ sports }}

      <br><br>

      <div>
        <label>Newslatter</label> <br>
        <input v-model="newslatter" type="radio" value="sim">Sim <br>
        <input v-model="newslatter" type="radio" value="não">Não
      </div>

      <br><br>

      {{ newslatter }}

    </div>
    -->
  </div>
  <!--FIM LIGAÇÃO DE DADOS (v-model)-->
  




  <!--DIRETRIZES-->
  <div>
    <!--
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
    -->
  </div>
  <!--FIM DIRETRIZES-->
</template>


<script>

  export default {
    name: 'App' ,
    data() {
      return {

        // CICLO DE VIDA (LIFE CYCLE)
        name: 'Maurício Casagrande'
        // FIM CICLO DE VIDA (LIFE CYCLE)




        // OBSERVADORES (WATCH)
        /*
        name: '',
        pageCount: 0,
        user: {
          firstName: '',
          lastName: ''
        }
        */
        // FIM OBSERVADORES (WATCH)




        // PROPRIEDADES COMPUTADAS
        /*
        user: {
          firstName: 'Maurício',
          lastName: 'Casagrande'
        },
        // FIM PROPRIEDADES COMPUTADAS
        */





        // LIGAÇÃO DE DADOS
        /*
        name: "",
        sports: "",
        newslatter: ""
        // FIM LIGAÇÃO DE DADOS
        */





        // DIRETRIZES
        /*
        classVar: "title",
        pClass: ['text', 'text-home'],
        isHome: true,
        */
        // FIM DIRETRIZES
        

        // RECURSO UTILIZADO EM AULA
        /*
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
        */
        
      }
    },

    methods: {

      // EVENTOS
      /*
      onClick($evt) {
        console.log('click', $evt);
      },

      onMouseOver($evt) {
        console.log('mouse over', $evt);
      },

      onMouseOut($evt) {
        console.log('mouse out', $evt);
      },

      onSubmit($evt) {
        console.log('submit', $evt);
      },

      onKeyUp($evt) {
        console.log('onKeyUp', $evt);
      }
      */
      // FIM EVENTOS





      // OBESERVADORES (WATCH)
      /*
      saveUserName() {
        console.log('Ajax');
        console.log(this.name);
      },

      changePage() {
        console.log('Ajax changePage');
      }
      */
      // FIM OBESERVADORES (WATCH)
    },

    computed: {
      // PROPRIEDADES COMPUTADAS
      /*
      fullName() {
        return `${this.user.firstName} ${this.user.lastName}`
      },

      // FILTRO
      unComletedTodos() {
        return this.todos.filter(a => !a.completed);
      },
      comletedTodos() {
        return this.todos.filter(a => a.completed);
      }
      */

    },

    watch: {

      // OBSERVADORES
      /*
      name(x) {
        if (x.length >= 3) {
          this.saveUserName();  
        }
      },

      pageCount() {
        this.changePage();
      },

      user: {
        // usa-se o  handler e deep para alterar os valores do objeto
        // exemplo, quero alterar o firsName e lastName e não o objeto user
        handler() {
          console.log('User alterado')
        },
        // observando profundamente (deep)
        deep: true
      }
      // FIM OBSERVADORES
      */
    },

    // CICLO DE VIDA DO COMPONENTE
    
    // H O O K S

    // antes de criar
    beforeCreate() {
      console.log('beforeCreate'); 
      console.log('Estado:', this.name);   
    },

    // depois de criado
    created() {
      console.log('created');
      console.log('Estado:', this.name);
    },

    // antes de ser montado
    beforeMount() {
      console.log('beforeMount');
      console.log('Estado:', this.name);
    },

    // depois de montado
    mounted() {
      console.log('mounted');
      console.log('Estado:', this.name);
    },

    // antes de desmontar
    beforeUnmount() {
      console.log('beforeUnmounted');
    },

    // desmontado
    unmounted() {
      console.log('unmounted');
    }
    // FIM CICLO DE VIDA DO COMPONENTE

  }

</script>



<style>
  /* .text {
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
  } */

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin: 60px;
  }
</style>
