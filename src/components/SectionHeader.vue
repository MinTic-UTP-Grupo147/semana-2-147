<template>
     <header>
            <nav class="navbar navbar-expand-lg sticky-top navbar-dark bg-dark ">
                <a class="navbar-brand " href="# ">
                    <img src="https://placeimg.com/30/30/any " width="30 " height="30
                    " class="d-inline-block align-top " alt=" " loading="lazy "> Grupo 147
                </a>
                <div class="flex navbar-collapse justify-content-end " id="navbarNav ">
                    <ul class="navbar-nav ">
                        <li class="nav-item active ">
                            <a class="nav-link " href="#">Inicio <span class="sr-only">(current)</span></a>
                        </li>
                        <li class="nav-item ">
                            <a class="nav-link " href="#services">Servicios</a>
                        </li>
                        <li class="nav-item ">
                            <a class="nav-link " href="#news">Noticias</a>
                        </li>
                        <li class="nav-item ">
                            <a class="nav-link " href="#team">Equipo</a>
                        </li>
                    </ul>
                </div>
            </nav>
            <!-- Imagen  carousel -->

            <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
                <ol class="carousel-indicators">
                    <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
                    <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
                    <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
                </ol>
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img src="https://placeimg.com/1000/300/animals" class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="https://placeimg.com/1000/300/nature" class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="https://placeimg.com/1000/300/any" class="d-block w-100" alt="...">
                    </div>
                </div>
                <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="sr-only">Previous</span>
                </a>
                <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="sr-only">Next</span>
                </a>
            </div>
        </header>    
</template>

<script>
export default {
    name: 'SectionHeader',
};
</script>