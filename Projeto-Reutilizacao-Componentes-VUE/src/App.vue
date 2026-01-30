<template> 
  <div>

    <Header/>
    <PrimeiroComponente/> <!-- Aqui o componente é utilizado -->
    <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
    <LifeCycle/>
    <Pessoa/>

  </div>
</template>

<script>

  import Header from './components/Header.vue';
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa  from './components/Pessoa.vue'

  export default{ //Exportando o componente como o Nome 'App' 
    name: 'App',
    components:{ //listando os componentes externos
      Header,
      PrimeiroComponente,
      LifeCycle,
      Pessoa
    },
    data(){
      return{
        testando: 'Teste'
      }
    }
  }

</script>

<style>
body{
  background-color: #333;
  color: #fff;

  }

  a {
    color:red;
  
  }

  .teste{
    background-color: black;

  }

</style>