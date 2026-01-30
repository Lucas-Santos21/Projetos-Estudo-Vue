<template>
    <div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    </div>
</template>

<script>

    export default{
        name: 'PrimeiroComponente',
        data(){ //função que manipula os dados do componente
            return{ //retorno dos dados do componente
                nome: 'Lucas', //dado definido
                profissao: 'Programador'
            }
        }
    }

</script>