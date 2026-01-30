<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem" /> <!--O emit está chamando o metodo de MudarImagem com outro nome para utiliza-lo -->
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue'

export default{
    name:'Picture',
    components:{
        MudarImagem
    },
    data(){
        return{
            avatar: "/img/avatar.png",
            descricao: "Lucas Santos"
        }
    },
    methods:{
        trocarImagem(){ //atribui uma funcionalidade para o metodo do outro componente(mudar o nome aqui nao interfere)
            this.avatar = "/img/avatar2.png"
        }
    }
}

</script>