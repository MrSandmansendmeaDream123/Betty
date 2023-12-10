<script setup>
import {ref} from 'vue'
defineProps(['id','title','body'])
const text = ref('')
const noteid = ref(0)

function edit() {
    text.value = 'edited'
}
</script>

<template>
    <div class="Note">
        <input type="checkbox" id="todo-item" />
        <label for="todo-note">Note</label>
        <div>
            <textarea id="todo-note">
            This is where the note will be
            </textarea>
        </div>
      
        
    </div>
</template>

