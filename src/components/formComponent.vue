<template>
    <div class="comp">
        <h1>{{ title }}</h1>
    </div>
</template>

<script>
    export default {
        name: "formComponent",
        data()
        {
            return{
                title: '#form component'
            }
        }
    }
</script>

<style scoped>

    .comp{
        background-color: yellow;
        border: 1px solid yellowgreen;
        margin: 5px;
        padding: 5px;
    }

</style>
