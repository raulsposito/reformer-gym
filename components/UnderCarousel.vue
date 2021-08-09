<template>
    <!-- This example requires Tailwind CSS v2.0+ -->
    <div class="relative bg-indigo-800">
    <div class="absolute inset-0">
        <img class="w-full h-full object-cover" :src="bgImage" alt="Pilates">
        <div class="absolute inset-0 bg-indigo-800 mix-blend-multiply" aria-hidden="true"></div>
    </div>
    <div class="relative max-w-7xl mx-auto py-24 px-4 sm:py-32 sm:px-6 lg:px-8">
        <h1 class="text-4xl font-extrabold tracking-tight text-white sm:text-5xl lg:text-6xl">Mejora tu calidad de vida.</h1>
        <p class="mt-6 text-xl text-indigo-100 max-w-3xl">Hacer ejercicio con el reformador es posible para cualquier persona, en cualquier nivel de forma física. No es de extrañar que el nombre completo del reformador sea reformador universal.</p>
    </div>
    </div>
</template>

<script>
    import bgImage from '../assests/horizontal.jpg'

    export default {
        data() {
            return {
                bgImage: bgImage
            }
        }
    }
</script>