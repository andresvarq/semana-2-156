<template>
                <div class="card text-white bg-dark">
                    <div class="d-flex justify-content-center p-2">
                        <img :src="member.imagen" alt="Fotografia del integrante">
                    </div>
                    <div class="card-body">
                        <h5 class="card-title">{{member.nombre}}</h5>
                        <p class="card-text">{{member.descripcion}}</p>
                        <p class="card-text"><span><b> Rol: </b></span>{{member.rol}}</p>
                        <p class="card-text"><span><b> Código: </b></span>{{member.codigo}}</p>

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
