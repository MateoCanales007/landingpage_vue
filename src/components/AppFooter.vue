<template>
    <v-footer class="text-center d-flex flex-column ga-2 py-4" color="indigo-lighten-1">
        <div class="d-flex ga-3">
            <v-btn v-for="icon in icons" :key="icon" :icon="icon" density="comfortable" variant="text"></v-btn>
        </div>

        <v-divider class="my-2" thickness="2" width="50"></v-divider>

        <div class="text-caption font-weight-regular opacity-60" id="footer-description">
            Vue.js es un framework progresivo para construir interfaces de usuario. Su núcleo se centra en la capa de vista, facilitando la integración con otras bibliotecas o proyectos existentes. Vue utiliza un sistema de reactividad eficiente y un DOM virtual para actualizaciones rápidas. Además, su ecosistema incluye herramientas como Vue Router y Vuex, permitiendo el desarrollo de aplicaciones SPA robustas y escalables. La comunidad de Vue es activa y ofrece abundantes recursos, documentación y componentes reutilizables.
        </div>

        <v-divider class="my-4" thickness="2" width="60" color="white"></v-divider>
        <div class="footer-bottom mt-2">
            {{ currentDate }} — <span class="footer-brand">Vuetify</span>
        </div>
    </v-footer>
</template>
<script setup>
import { ref } from 'vue'
// Puedes personalizar los íconos aquí:
const icons = [
    'mdi-facebook',
    'mdi-twitter',
    'mdi-linkedin',
    'mdi-instagram',
]
const currentDate = ref(
    new Date().toLocaleDateString('es-ES', {
        day: '2-digit',
        month: '2-digit',
        year: '2-digit'
    })
)
</script>

<style scoped>
.footer-custom {
    background: linear-gradient(90deg, #5c6bc0 0%, #3949ab 100%);
    color: #fff;
    border-top-left-radius: 24px;
    border-top-right-radius: 24px;
    box-shadow: 0 -2px 16px rgba(60, 60, 120, 0.12);
}

#footer-description {
    max-width: 800px;
    font-size: 1.1rem;
    color: #e0e0e0;
    font-weight: 400;
    margin: 0 auto;
}

.footer-icon {
    transition: transform 0.2s, box-shadow 0.2s;
    box-shadow: 0 2px 8px rgba(60, 60, 120, 0.10);
}

.footer-icon:hover {
    transform: scale(1.15);
    box-shadow: 0 4px 16px rgba(60, 60, 120, 0.18);
}

.footer-description {
    max-width: 800px;
    font-size: 1.1rem;
    color: #e0e0e0;
    font-weight: 400;
}

.footer-bottom {
    font-size: 1.3rem;
    font-weight: 400;
    color: #fff;
}

.footer-brand {
    font-weight: bold;
    color: #ffffff;
    letter-spacing: 1px;
}
</style>