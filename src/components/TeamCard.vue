<template>

    <div class="card text-white" style="background-color: rgba(255, 255, 255, 0.3)">
        <div class="d-flex justify-content-center p-2 media">
            <img v-bind:src='member.image' alt="Foto miembro del equipo" width="190em" height="190em" style="border-radius: 15%">
        </div>
        <div class="card-body">
            <h5 class="card-title">{{ member.nombre }}</h5>
            <p class="card-text">({{ member.codigo }}) {{ member.rol }}</p>
            <p class="card-text">{{ member.descripcion }}</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
