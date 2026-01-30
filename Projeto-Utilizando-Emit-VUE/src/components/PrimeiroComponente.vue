<template>
    <div>
    <Reutilizacao />
    <h1>Olá Vue!</h1>
    <Reutilizacao />
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <MultiplosEventos />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
import Reutilizacao from './Reutilizacao.vue';

    export default{
        name: 'PrimeiroComponente',
        components:{
            MultiplosEventos,
            Reutilizacao
        },
        data(){ //função que manipula os dados do componente
            return{ //retorno dos dados do componente
                nome: 'Lucas', //dado definido
                profissao: 'Programador'
            }
        }
    }

</script>