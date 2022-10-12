<template>
    <div class="main-content" >
        <h1>Content Component</h1>
        <p>Mostrar resultado de: 2 + 2 = {{2+2}}</p>
        <p>Mostrar string con una función: {{showstring()}}</p>
        <p v-if="show">Este texto solo se muestra si la variable show es true</p>
        <button @click="toggle" class="mt-5">Show Text</button>
        <button @click="changeColor" class="mt-5" :style="`background-color: ${arrayColores[i]}`">Change style</button>

    </div>
</template>
  
<script setup>
import { ref } from "vue";

const showstring = () => {
    return "Hello World"
}

let show = ref(false);

const toggle = () => {
    show.value = !show.value;
}

const arrayColores = ["blue", "green", "yellow", "red"]
let i = ref(0);
const changeColor = () => {
i.value++;
if(i.value > 3) i.value = 0
}


</script>
<style scoped>
.main-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 5rem;

}

</style>