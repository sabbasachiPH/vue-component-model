<script setup>

const props = defineProps(['person']);

</script>

<template>
    <h3 class="text-3xl ">Child Components</h3>
    <div>
        <p>
            <label>Name - {{ person.name }}</label> <br />
            <input v-model="person.name" class="mx-auto p-5 m-5 text-xl text-black" type="text">
        </p>
        <p>
            <label>Email - {{ person.email }}</label> <br />
            <input v-model="person.email" class="mx-auto p-5 m-5 text-xl text-black" type="text">
        </p>
    </div>
</template>



<style scoped></style>