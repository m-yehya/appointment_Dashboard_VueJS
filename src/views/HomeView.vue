<template>
  <div class="q-pa-md">
    <q-toolbar class="q-ma-sm">
      <q-input
        outlined
        v-model="text"
        label="Search"
        :dense="dense"
        rounded
        class="search"
      >
        <template v-slot:append>
          <q-icon name="search" />
        </template>
      </q-input>
      <q-space></q-space>
      <q-btn color="white" text-color="black" icon="fas fa-moon" />
    </q-toolbar>
    <q-toolbar>
      <h6 class="text-weight-bolder">Dashboard</h6>
      <q-space></q-space>
      <q-icon name="fas fa-calendar-minus" size="" class="q-mr-sm" />
      <div class="text-overline">Wednesday, 21.03.2022</div>
    </q-toolbar>
    <div class="row q-col-gutter-md top">
      <div class="col-3">
        <PatientsNumber/>
      </div>
      <div class="col-3">
        <NewPatients/>
        <OldPatients/>
      </div>
      <div class="col-6">
        <PatientsStatistics/>
      </div>
    </div>
    <q-toolbar>
      <div class="text-overline">Events</div>
      <q-space></q-space>

      <div class="text-overline">Your patients today</div>
      <div class="text-caption text-green q-ml-md">All patients</div>
      <q-icon
        name="fas fa-chevron-right"
        size="10px"
        class=""
        color="green-7"
      />
    </q-toolbar>
    <div class="row q-col-gutter-md">
      <div class="col-6">
        <DailyEvents/>
      </div>
      <div class="col-6">
        <TodayPatient/>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import { ref } from "vue";
import NewPatients from "@/components/NewPatients.vue";
import OldPatients from "@/components/OldPatients.vue"
import PatientsNumber from "@/components/PatientsNumber.vue"
import PatientsStatistics from "@/components/PatientsStatistic.vue"
import DailyEvents from "@/components/DailyEvents.vue"
import TodayPatient from "@/components/TodayPatient.vue"
// import { shuffle } from "lodash";

export default {
  name: "HomeView",
  components: {
    NewPatients,
    OldPatients,
    PatientsNumber,
    PatientsStatistics,
    DailyEvents,
    TodayPatient,
  },

  setup() {
    return {
      slide: ref("style"),
      lorem: "Lorem ipsum dolor, sit amet consectetur adipi.",
    };
  },
};
</script>
<style scoped>
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