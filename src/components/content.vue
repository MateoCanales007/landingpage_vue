<template>
  <div
    class="curiosidades-vue p-6 max-w-3xl mx-auto bg-white rounded-2xl shadow-lg"
  >
    <h1 class="text-3xl font-bold text-green-600 mb-4">¿Qué es Vue.js?</h1>
    <p class="mb-6 text-gray-700">
      Vue.js es un <strong>framework progresivo de JavaScript</strong> utilizado
      para crear interfaces de usuario interactivas. Su enfoque es incremental,
      lo que significa que puedes usarlo en una parte pequeña de tu aplicación o
      para construir proyectos completos. Gracias a su simplicidad y
      flexibilidad, se ha convertido en una de las herramientas favoritas para
      desarrolladores frontend en todo el mundo.
    </p>

    <img
      src="../assets/logo.png"
      alt="Logo de Vue.js"
      class="mb-4 rounded-lg shadow first-logo"
    />

    <h1 class="text-2xl font-semibold mb-3" id="curiosidades-t">
      Curiosidades sobre Vue.js
    </h1>
    <ul class="list-disc pl-6 space-y-4 text-gray-700">
      <li>
        <h2>1. Creado por un exempleado de Google</h2>
        Vue fue desarrollado por Evan You en 2014, quien antes había trabajado
        en Google usando AngularJS. Su idea era tomar lo mejor de Angular y
        hacerlo mucho más ligero y sencillo.
      </li>
      <img
        src="https://images.ctfassets.net/s5uo95nf6njh/5PpFIeuDxz2T89nZNED1EP/48d62a69f31a3ab6dfc58938eb7b8c2a/evan-you-portrait.jpg?w=1200&fm=jpg"
        alt="Evan you"
        class="mb-6 rounded-lg shadow"
      />

      <li>
        <h2>2. Es mantenido principalmente por la comunidad</h2>
        Aunque Vue tiene un creador principal, la mayor parte de su evolución se
        debe a colaboradores de todo el mundo. Hoy en día cuenta con miles de
        “contribuidores” en GitHub.
        <!-- 🔽 Imagen idea: captura de la página de Vue en GitHub -->
      </li>
      <img
        src="https://miro.medium.com/1*yZYh6z26VwWbinUYV8ymLQ.png"
        class="mb-6 rounded-lg shadow"
      />

      <li>
        <h2>3. Popular en Asia y Europa</h2>
        Aunque React domina en Estados Unidos, Vue tiene gran aceptación en
        países asiáticos como China y Japón, y en varias partes de Europa.
        Grandes empresas como Alibaba, Xiaomi y GitLab lo utilizan.
      </li>
      <img
        src="https://blog.boon.so/wp-content/uploads/2024/03/Alibaba-Logo-3.png"
        class="mb-6 rounded-lg shadow"
      />
    </ul>

    <p class="mt-6 text-gray-700">
      En resumen, Vue.js no solo es fácil de aprender, sino que además cuenta
      con una comunidad vibrante y casos de éxito en empresas de todo el mundo.
      Si buscas una herramienta flexible y poderosa, Vue es una gran elección.
    </p>
  </div>
</template>

<script>
export default {
  name: "CuriosidadesVue",
};
</script>

<style scoped>
.curiosidades-vue {
  font-family: "Inter", sans-serif;
}
img.first-logo {
  border: none;
  width: 150px;
}
#curiosidades-t {
  color: white;
  background-color: rgb(0, 128, 92);
  padding: 15px;
  width: 100%;
  margin: 0;
}
img {
  width: 300px;
  margin: 5%;
  border: solid 3px rgb(173, 142, 142);
  border-radius: 15px;
}
.curiosidades-vue {
  margin: 0%;

  padding: 5%;
  text-align: center;
  background-color: rgb(219, 217, 217);
  color: rgb(0, 0, 0);
}
.curiosidades-vue li {
  text-align: left;
}
</style>
