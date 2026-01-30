<template>
    <div>
        <h2>Meu Formulário</h2>
        <form action="">
            <div>
            <InputText/>
            </div>
            <div>
            <InputText/>
            </div>
            <div>
            <Submit/>
            </div>
        </form>

    </div>
</template>

<script>

import InputText from './form/InputText.vue'
import Submit from './form/submit.vue'

export default{
    name: 'Form',
    components:{
        InputText,
        Submit
    }
}

</script>