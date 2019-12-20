<template>
    <div class="comp">
        <h1> {{ title }} </h1>
        <p>ao</p>
        <span>curso de {{ msg }}</span>
    </div>
</template>

<script>
    export default {
        name: "teste-component",
        data()
        {
            return{
                title: 'teste Component',
                msg: 'VueJs'
            }
        }
    }
</script>

<style scoped>

    .comp{
        width: 98%;
        background-color: crimson;
        border: 1px solid purple;
        margin: 5px;
        padding: 5px;
    }
</style>
