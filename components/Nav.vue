<template>
    <header class="bg-secondary">
    <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8" aria-label="Top">
        <div class="w-full py-6 flex items-center justify-between border-b border-secondary lg:border-none">
        <div class="flex items-center">
            <a href="/">
            <span class="sr-only">Essence</span>
            <img class="h-10 w-auto" :src="logo" alt="">
            </a>
            <div class="hidden ml-10 space-x-8 lg:block">
            <a href="/reformer" class="text-base font-medium text-white hover:text-indigo-50" key="Solutions">
                Que es Pilates Reformer?
            </a>

            <a href="/planes" class="text-base font-medium text-white hover:text-indigo-50" key="Pricing">
                Nuestros planes
            </a>

            <a href="/contacto" class="text-base font-medium text-white hover:text-indigo-50" key="Docs">
                Contacto
            </a>
            </div>
        </div>
        <!-- <div class="ml-10 space-x-4">
            <a href="#" class="inline-block bg-indigo-500 py-2 px-4 border border-transparent rounded-md text-base font-medium text-white hover:bg-opacity-75">Sign in</a>
            <a href="#" class="inline-block bg-white py-2 px-4 border border-transparent rounded-md text-base font-medium text-indigo-600 hover:bg-indigo-50">Sign up</a>
        </div> -->
        </div>
        <div class="py-4 flex flex-wrap justify-center space-x-6 lg:hidden">
        <a href="/reformer" class="text-base font-medium text-white hover:text-indigo-50" key="Solutions">
            Que es Pilates Reformer?
        </a>

        <a href="/planes" class="text-base font-medium text-white hover:text-indigo-50" key="Pricing">
            Nuestros planes
        </a>

        <a href="/contacto" class="text-base font-medium text-white hover:text-indigo-50" key="Docs">
            Contacto
        </a>
        </div>
    </nav>
    </header>
</template>

<script>
    import logo from '../assests/EssenseIso.JPG'

    export default {
        data() {
            return {
                logo: logo
            }
        }
    }
</script>