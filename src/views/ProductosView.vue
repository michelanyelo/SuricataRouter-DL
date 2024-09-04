<template>
    <section class="container" id="productos">
        <h1 class="text-center">Productos</h1>
        <div class="row">
            <div class="col-sm-4 col-12 px-5 mb-4" v-for="(card, id) in cards" :key="id">
                <SingleCard :nombre="card.nombre" :descripcion="card.descripcion" :precio="card.precio"
                    :porcion="card.porcion" />
            </div>
        </div>
        <button class="btn btn-warning mt-2" @click="volverInicio"><i class="fa-solid fa-house me-2"></i>Inicio</button>
    </section>
</template>

<script setup>
import SingleCard from '../components/SingleCard.vue'
import { useRouter } from 'vue-router'

const router = useRouter()
const cards = [
    {
        id: 1,
        nombre: 'Colaciones',
        descripcion: 'Porotos con riendas',
        precio: '$4990',
        porcion: 'Para 1 persona'
    }
]

const volverInicio = () => {
    router.push({ name: 'home' })
}

</script>