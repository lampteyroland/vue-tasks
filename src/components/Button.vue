<template>
    <div>
        <button @click="onClick" :style="{backgroundColor: color}" class="btn">{{ text }}</button>

    </div>
</template>

<script>
    export default {
    name: 'Button',        
    props:{
       text: String,    
       color: String

       },
       methods:{
        onClick(){
            this.$emit('btn-click')
       }

       }
    }
</script>

<style  scoped>

</style>