<template>
    <div class="relative py-16 bg-white overflow-hidden">
    <div class="hidden lg:block lg:absolute lg:inset-y-0 lg:h-full lg:w-full">
        <div class="relative h-full text-lg max-w-prose mx-auto" aria-hidden="true">
        <svg class="absolute top-12 left-full transform translate-x-32" width="404" height="384" fill="none" viewBox="0 0 404 384">
            <defs>
            <pattern id="74b3fd99-0a6f-4271-bef2-e80eeafdf357" x="0" y="0" width="20" height="20" patternUnits="userSpaceOnUse">
                <rect x="0" y="0" width="4" height="4" class="text-gray-200" fill="currentColor" />
            </pattern>
            </defs>
            <rect width="404" height="384" fill="url(#74b3fd99-0a6f-4271-bef2-e80eeafdf357)" />
        </svg>
        <svg class="absolute top-1/2 right-full transform -translate-y-1/2 -translate-x-32" width="404" height="384" fill="none" viewBox="0 0 404 384">
            <defs>
            <pattern id="f210dbf6-a58d-4871-961e-36d5016a0f49" x="0" y="0" width="20" height="20" patternUnits="userSpaceOnUse">
                <rect x="0" y="0" width="4" height="4" class="text-gray-200" fill="currentColor" />
            </pattern>
            </defs>
            <rect width="404" height="384" fill="url(#f210dbf6-a58d-4871-961e-36d5016a0f49)" />
        </svg>
        <svg class="absolute bottom-12 left-full transform translate-x-32" width="404" height="384" fill="none" viewBox="0 0 404 384">
            <defs>
            <pattern id="d3eb07ae-5182-43e6-857d-35c643af9034" x="0" y="0" width="20" height="20" patternUnits="userSpaceOnUse">
                <rect x="0" y="0" width="4" height="4" class="text-gray-200" fill="currentColor" />
            </pattern>
            </defs>
            <rect width="404" height="384" fill="url(#d3eb07ae-5182-43e6-857d-35c643af9034)" />
        </svg>
        </div>
    </div>
    <div class="relative px-4 sm:px-6 lg:px-8">
        <div class="text-lg max-w-prose mx-auto">
        <h1>
            <span class="block text-base text-center text-secondary font-semibold tracking-wide uppercase">Que es?</span>
            <span class="mt-2 block text-3xl text-center leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">Pilates Reformer</span>
        </h1>
        <p class="mt-8 text-xl text-gray-500 leading-8">Este ejercicio para todo el cuerpo recluta todas las fibras musculares, lo que conduce a un núcleo más fuerte. Ayuda con la estabilidad y el equilibrio de las articulaciones y fortalece los abdominales, glúteos e isquiotibiales. Estos sostienen la columna y alargan los flexores de la cadera, lo que aumenta la flexibilidad y mejora la postura.</p>
        </div>
        <div class="text-lg max-w-prose mx-auto">
        <h1>
            <span class="block pt-16 text-base text-center text-secondary font-semibold tracking-wide uppercase">Es apto para todo tipo de personas</span>
            <span class="mt-2 block text-3xl text-center leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">Recomendado para:</span>
        </h1>
        <p class="mt-8 text-xl text-gray-500 leading-8">
            <ul>
                <li>* Personas con dolencias de espalda o postura.</li>
                <li>* Personas con movilidad reducida.</li>
                <li>* Deportistas con lesiones.</li>
            </ul>
        </p>
        </div>
        <div class="mt-16 prose prose-indigo prose-lg text-gray-500 mx-auto">
        <figure>
            <img class="w-full max-h-screen object-cover rounded-lg pt-8" :src="img" alt="Nuestro Gimnasio">
            <figcaption>Conoce nuestro gimnasio personalizado en Solymar.</figcaption>
        </figure>
        </div>
    </div>
    </div>
</template>

<script>
    import img from '../assests/img1.jpg'

    export default {
        data() {
            return {
                img: img
            }
        }
    }
</script>