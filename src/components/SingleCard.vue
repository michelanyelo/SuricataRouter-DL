<template>
    <div class="card">
        <img src="../assets/img/colaciones.jpg" class="card-img-top" alt="colaciones" />
        <div class="card-body">
            <h5 class="card-title fw-bold">{{ nombre }}</h5>
            <p class="card-text">{{ descripcion }}</p>
        </div>
        <ul class="list-group list-group-flush">
            <li class="list-group-item">Precio: {{ precio }}</li>
            <li class="list-group-item">Porcion: {{ porcion }}</li>
        </ul>
        <div class="card-body">
            <a href="#" class="card-link">Ver más</a>
            <a href="#" class="card-link">Comprar</a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardComp',
    props: {
        nombre: {
            type: String,
            required: true
        },
        descripcion: {
            type: String,
            required: true
        },
        precio: {
            type: String,
            required: true
        },
        porcion: {
            type: String,
            required: true
        }
    }
}
</script>

<style></style>