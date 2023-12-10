<script setup>
import { onBeforeMount } from 'vue';
import Note from "./Note.vue";
    onBeforeMount(() => {
        fetch('http://localhost:3000/notes/', {
        method: 'GET'
        })
        .then(res => res.json())
        .then(
        json => console.log(JSON.stringify(json))
        // or whatever you need to do
        )
    })
    
</script>

<template>
    <div class="white-board">
        <Note />
    </div>
</template>