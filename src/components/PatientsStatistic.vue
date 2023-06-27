<template>
    <q-card class="q-mx-md q-pa-md doctors" bordered>
          <div class="text-overline">Statistic</div>
          <div class="">
            <q-carousel
              v-model="slide"
              vertical
              transition-prev="slide-down"
              transition-next="slide-up"
              swipeable
              animated
              control-color="green-7"
              navigation-icon="radio_button_unchecked"
              navigation
              padding
              arrows
              height="160px"
              class="text-black shadow-1 rounded-borders"
            >
              <q-carousel-slide name="style" class="column no-wrap flex-center">
                <q-icon name="style" size="36px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide name="tv" class="column no-wrap flex-center">
                <q-icon name="live_tv" size="36px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide
                name="layers"
                class="column no-wrap flex-center"
              >
                <q-icon name="layers" size="36px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
            </q-carousel>
          </div>
        </q-card>
  </template>
  
  <script>
  import { ref } from "vue";

  export default {
    setup() {
    return {
      slide: ref("style"),
      lorem: "Lorem ipsum dolor, sit amet consectetur adipi.",
     
    };
  },
  }
  </script>
  
  <style>
  
  </style>