<template>
    <h2>v-modelは、初期化した変数msgを画面から変更し、即座に反映できる</h2>
    <div>はじめの変数modelMSG:初期MSG</div>
    <div>inputで書き換えると、modelMSG変数に代入:{{modelMSG}}</div>
    <input v-model="modelMSG">
</template>

<script>
export default {
    name:"V_model",
    data(){
        return{
            modelMSG:"初期MSG"
        } 
    }
}
</script>