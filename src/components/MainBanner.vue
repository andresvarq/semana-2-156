<template>

<div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators">
        <li data-target="#carouselExampleCaptions" data-slide-to="0" class=""></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
    </ol>
    <div class="carousel-inner">
        <div class="carousel-item">
            <img src='./components/img/soccer-field-drawn-on-blackboard-min.jpg' alt="" width="100%" height="400">
            <div class="carousel-caption d-none d-md-block" style="color: #f51720;">
                <h5>Mi Equipo</h5>
                <p>La información de tu equipo favorito rápido y al instante.</p>
            </div>
        </div>
        <div class="carousel-item">
            <img src='./components/img/26141-min.jpg' alt="" width="100%" height="400">
            <div class="carousel-caption d-none d-md-block" style="color: #f51720;">
                <h5>Proximas fechas</h5>
                <p>Toda la emoción de los siguientes partidos.</p>
            </div>
        </div>
        <div class="carousel-item">
            <img src='./components/img/vector-campo-futbol-verde-o-campo-futbol-parrilla_1284-41290-min.jpg' alt="" width="100%" height="400">
            <div class="carousel-caption d-none d-md-block" style="color: #f51720;">
                <h5>Staff</h5>
                <p>Conoce a nuestro staff de miembros.</p>
            </div>
        </div>
    </div>
    <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
</div>

</template>

<script>
export default {
    name: 'MainBanner'
}
</script>