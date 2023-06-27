<template>
    <q-card class="q-mx-md q-pa-sm" bordered>
          <div class="row q-col-gutter-md">
            <div class="col-3">
              <div class="text-caption text-weight-bolder q-mt-lg">
                10:00 am
              </div>
            </div>
            <div class="col-9">
              <q-card class="q-px-sm colorCard" bordered flat>
                <q-item>
                  <q-item-section avatar>
                    <q-avatar>
                      <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
                    </q-avatar>
                  </q-item-section>

                  <q-item-section>
                    <q-item-label>Sarah Hosten</q-item-label>
                    <q-item-label caption>Diagnosis: Stroke</q-item-label>
                  </q-item-section>
                  <q-item-section side>
                    <q-icon name="fas fa-ellipsis-v" color="" />
                  </q-item-section>
                </q-item>
              </q-card>
            </div>
          </div>
          <div class="row q-col-gutter-md q-mt-md">
            <div class="col-3">
              <div class="text-caption text-weight-bolder q-mt-lg">
                10:00 am
              </div>
            </div>
            <div class="col-9">
              <q-card class="q-px-sm colorCard" bordered flat>
                <q-item>
                  <q-item-section avatar>
                    <q-avatar>
                      <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
                    </q-avatar>
                  </q-item-section>

                  <q-item-section>
                    <q-item-label>Sarah Hosten</q-item-label>
                    <q-item-label caption>Diagnosis: Stroke</q-item-label>
                  </q-item-section>
                  <q-item-section side>
                    <q-icon name="fas fa-ellipsis-v" color="" />
                  </q-item-section>
                </q-item>
              </q-card>
            </div>
          </div>
        </q-card>
  </template>
  
  <script>
  export default {
  
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