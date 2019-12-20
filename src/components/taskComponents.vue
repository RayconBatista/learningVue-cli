<template>
    <div class="comp">
        <h1>{{title}}</h1>
        <table class="borderTable">
            <tr>
                <th>nome</th>
                <th>Completa?</th>
            </tr>
            <tr v-for="(task, index) in tasks" :key="index">
                <td>{{ task.name }}</td>
                <td>{{ task.completed ? 'Sim' : 'Não'}}</td>
            </tr>
        </table>
    </div>
</template>

<script>
    export default {
        name: "taskComponents",
        data()
        {
            return{
                tasks:[
                    {name: 'Lavar louça', completed: false},
                    {name: 'Lavar banheiro', completed: true},
                    {name: 'Lavar carro', completed: false},
                    {name: 'Lavar moto', completed: true},
                ],
                title: 'Tasks Components'
            }
        }
    }
</script>

<style scoped>
    .comp{
        background-color: dodgerblue;
        border: 1px solid green;
        width: 15vw;
    }

    table.borderTable{
        border-collapse: collapse;
        background: aliceblue;
    }

    table.borderTable td{
        border: 1px solid black;
    }

    table.borderTable th{
        border: 1px solid black;
    }
</style>
