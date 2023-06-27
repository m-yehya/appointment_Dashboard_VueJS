<template>
 <q-card class="q-mx-md" bordered>
          <div class="flex flex-center column">
            <q-circular-progress
              show-value
              font-size="12px"
              value="70"
              size="100px"
              :thickness="0.22"
              color="green-7"
              track-color="green-2"
              class="q-ma-md"
            >
              784 Patients
            </q-circular-progress>
            <div>
              <q-badge color="green-2" rounded class="q-mr-sm" />Woman 40%
            </div>
            <div class="q-mb-xl">
              <q-badge color="green-7" rounded class="q-mr-sm" />Man 60%
            </div>
          </div>
        </q-card>
  </template>
  
  <script>
  export default {
  
  }
  </script>
  
  <style>
  
  </style>