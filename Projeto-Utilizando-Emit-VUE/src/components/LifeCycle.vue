<template>

<h1>Meu nome é: {{ nome }}</h1>

</template>

<script>

export default{
    name:'LifeCycle',
    data(){
        return{
            nome: 'Ainda nao sei'
        }
    },
    created(){ //O hook created acontece quando o Vue já criou o componente na memória, mas ainda não colocou o HTML na tela.
        setTimeout(() =>{
            this.nome = 'Lucas'
        }, 1000)

        this.lifeCycle()
    },
    mounted(){ //Já o hook mounted acontece quando o componente está na tela com html, dom e tudo funcionando.
        setTimeout(() =>{ 
            this.nome = 'Pedro'
        }, 2000);

        this.lifeCycle()
        
    },
    methods: {
        lifeCycle(){
            console.log("Executou");
        }
    }
}

</script>

