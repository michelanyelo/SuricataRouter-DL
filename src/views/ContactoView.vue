<template>
    <div class="contacto">

        <div class="container">
            <div class="d-flex align-items-center">
                <i class="fa-regular fa-envelope fs-1 me-3"></i>
                <h1 class="text-uppercase">Contacto</h1>
            </div>
            <form>
                <div class="mb-3">
                    <label for="inputEmail" class="form-label">Correo electrónico</label>
                    <input type="email" class="form-control" id="inputEmail" aria-describedby="emailHelp" required>
                </div>
                <div class="mb-3">
                    <label for="textMensaje" class="form-label">Felicitaciones / Sugerencias / Reclamos</label>
                    <textarea class="form-control" id="textMensaje" required></textarea>
                </div>
                <div class="mb-3 form-check">
                    <input type="checkbox" class="form-check-input" id="checkCondiciones" required>
                    <label class="form-check-label" for="checkCondiciones">¿Está de acuerdo con las
                        condiciones??</label>
                </div>
                <button type="submit" class="btn btn-primary">Submit</button>
            </form>
        </div>
    </div>
</template>
<style scoped></style>