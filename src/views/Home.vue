<template>
  <div class="home">
    <div class="calendar">
      <div class="calendar__header">
        <h1>October</h1>
      </div>
      <div class="calendar__body">
        <div class="calendar__body--days flex flex-wrap">
          <div
            v-for="(day, i) in days"
            :key="i"
            class="day border-solid border-gray-300 border w-40 h-40"
          >
            <p>{{ day }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      days: 31,
    };
  },
};
</script>
