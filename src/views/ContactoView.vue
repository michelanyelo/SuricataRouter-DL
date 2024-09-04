<template>
    <div class="contacto">
        <div class="container">
            <div class="d-flex align-items-center">
                <i class="fa-regular fa-envelope fs-1 me-3"></i>
                <h1 class="text-uppercase">Contacto</h1>
            </div>
            <form>
                <div class="mb-3">
                    <label for="inputEmail" class="form-label">Correo electrónico*</label>
                    <input type="email" class="form-control" id="inputEmail" aria-describedby="emailHelp" required>
                </div>
                <div class="mb-3">
                    <label for="selectMotivo" class="form-label">Motivo de contacto*</label>
                    <select class="form-select" aria-label="Default select example">
                        <option selected disabled>Seleccionar motivo</option>
                        <option value="1">Sugerencia</option>
                        <option value="2">Reclamo</option>
                        <option value="3">Felicitaciones</option>
                    </select>
                </div>
                <div class="mb-3">
                    <label for="textMensaje" class="form-label">Comentarios*</label>
                    <textarea class="form-control" id="textMensaje" required></textarea>
                </div>
                <div class="mb-3 form-check">
                    <input type="checkbox" class="form-check-input" id="checkCondiciones" required>
                    <label class="form-check-label" for="checkCondiciones">Estoy de acuerdo con las
                        condiciones*</label>
                </div>
                <button type="submit" class="btn btn-primary"><i
                        class="fa-regular fa-paper-plane me-2"></i>Enviar</button>
            </form>
            <button class="btn btn-warning mt-2" @click="volverInicio"><i
                    class="fa-solid fa-house me-2"></i>Inicio</button>
        </div>
    </div>
</template>
<script setup>
import { useRouter } from 'vue-router'

const router = useRouter()
const volverInicio = () => {
    router.push({ name: 'home' })
}
</script>
<style scoped>
.form-label,
.form-check-label {
    font-size: 16px;
    font-weight: bold;
    text-transform: uppercase;
}
</style>