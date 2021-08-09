<template>
  <main>
    <div>
      <div>
        <div class="h-auto">
            <carousel
                ref="Carousel"
                :per-page="1"
                :mouse-drag="false"
                :pagination-enabled="false"
                :navigation-enabled="false"
                :autoplay="true"
                :loop="true"
                :speed="2000"
                :autoplay-timeout="9000"
            >
                <slide
                v-for="(place, index) in places"
                :key="place.title"
                :index="index"
                class="h-full"
                >
                <div
                    id="me"
                    class="relative h-96 bg-gray-300 mix-blend-multiply"
                >
                    <div class="relative inset-0 z-10">
                    <h1
                        class="pt-10 text-center text-4xl font-semibold tracking-tight sm:text-5xl lg:text-6xl"
                    >
                        <!-- <span class="block text-white">{{ place.title }}</span>
                        <span class="block text-indigo-200">
                        {{ place.area }} · {{ place.plan }}
                        </span> -->
                    </h1>
                    </div>
                    <div class="absolute inset-0 z-5">
                    <img
                        class="h-full min-w-full object-cover"
                        :src="place.image_url"
                    />
                    </div>
                </div>
                </slide>
            </carousel>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel'
export default {
  components: {
    Carousel,
    Slide,
  },
  data() {
    return {
      places: [
        {
          index: 0,
          image_url: require('../assests/img1.jpg'),
        },
        {
          index: 1,
          image_url: require('../assests/1.jpg'),
        },
      ],
    }
  },
  methods: {
    nextSlide() {
      this.$refs.Carousel.goToPage(
        this.$refs.Carousel.getNextPage(),
        (this.$refs.scrollLBtn.disabled = false)
      )
      if (this.$refs.Carousel.canAdvanceBackward === false)
        this.$refs.scrollLBtn.disabled = true
      if (this.$refs.Carousel.canAdvanceForward === false)
        this.$refs.scrollRBtn.disabled = true
    },
    prevSlide() {
      this.$refs.Carousel.goToPage(
        this.$refs.Carousel.getPreviousPage(),
        (this.$refs.scrollRBtn.disabled = false)
      )
      if (this.$refs.Carousel.canAdvanceForward === false)
        this.$refs.scrollRBtn.disabled = true
      if (this.$refs.Carousel.canAdvanceBackward === false)
        this.$refs.scrollLBtn.disabled = true
    },
  },
}
</script>

<style>
#me {
  height: 40rem;
}
</style>
