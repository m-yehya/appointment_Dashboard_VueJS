<template>
    <q-card class="card1 q-mx-md q-pa-sm" bordered>
          <div class="row q-col-gutter-md">
            <div class="col-6">
              <div class="text-caption">Team meeting</div>
              <div class="text-caption text-grey-5">13:30 - 14:30</div>
              <div>
                <q-avatar
                  v-for="n in 5"
                  :key="n"
                  size="40px"
                  class="overlapping"
                  :style="`left: ${n * 25}px`"
                >
                  <img :src="`https://cdn.quasar.dev/img/avatar${n + 1}.jpg`" />
                </q-avatar>
              </div>
            </div>
            <div class="col-6">
              <div class="flex justify-end row">
                <q-toggle color="green" v-model="selection" val="green" />
              </div>
              <div class="flex justify-end row">
                <q-btn
                  round
                  icon="fas fa-pencil-alt"
                  size="10px"
                  color="black"
                  class="q-mr-sm"
                ></q-btn>
                <q-btn
                  round
                  icon="fas fa-chevron-right"
                  size="10px"
                  color="green"
                ></q-btn>
              </div>
            </div>
          </div>
        </q-card>
        <q-card class="card1 q-mx-md q-pa-sm q-mt-sm" bordered>
          <div class="row q-col-gutter-md">
            <div class="col-6">
              <div class="text-caption">Nobel prize</div>
              <div class="text-caption text-grey-5">13:30 - 14:30</div>
              <div>
                <q-avatar
                  v-for="n in 5"
                  :key="n"
                  size="40px"
                  class="overlapping"
                  :style="`left: ${n * 25}px`"
                >
                  <img :src="`https://cdn.quasar.dev/img/avatar${n + 1}.jpg`" />
                </q-avatar>
              </div>
            </div>
            <div class="col-6">
              <div class="flex justify-end row">
                <q-toggle color="gre" v-model="selection" val="" />
              </div>
              <div class="flex justify-end row">
                <q-btn
                  round
                  icon="fas fa-pencil-alt"
                  size="10px"
                  color="black"
                  class="q-mr-sm"
                ></q-btn>
                <q-btn
                  round
                  icon="fas fa-chevron-right"
                  size="10px"
                  color="green"
                ></q-btn>
              </div>
            </div>
          </div>
        </q-card>
  </template>
  
  <script>
  import { ref } from "vue";
  export default {
    setup() {
    return {
      
      selection: ref(["green"]),
    };
  },
  }
  </script>
  
  <style>
  .search {
  width: 700px;
}
.doctors {
  height: 220px;
}
.overlapping {
  border: 2px solid white;
  position: absolute;
  margin-left: -20px;
}
.card1 {
  height: 100px;
}
.top {
  margin-top: -40px;
}
.colorCard {
  background: #f8f8f8;
}
  </style>