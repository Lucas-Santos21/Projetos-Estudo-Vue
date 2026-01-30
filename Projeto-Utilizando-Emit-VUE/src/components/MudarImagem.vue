<template>
    <div>
        <button @click="$emit('mudarImagem')">Trocar Imagem de perfil</button>
    </div>
</template>

<script>
    export default{
        name: 'MudarImagem',
        emits: ['mudarImagem'] //esta enviando pro outro componente q possui um metodo q pode ser implementado
    }
</script>