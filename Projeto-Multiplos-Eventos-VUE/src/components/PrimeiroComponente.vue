<template>
    <div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <MultiplosEventos />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';

    

    export default{
        name: 'PrimeiroComponente',
        components:{
            MultiplosEventos
        },
        data(){ //função que manipula os dados do componente
            return{ //retorno dos dados do componente
                nome: 'Lucas', //dado definido
                profissao: 'Programador'
            }
        }
    }

</script>