<template>
  <div class="event-card">
    <!--en este div encontraremos los datos del evento-->
    <span>@ {{ event.time }} en {{ event.date }}</span>
    <h4>{{ event.title }}</h4>
  </div>
</template>

<script>
export default {
  name: "EventCard",
  props: {
    event: Object
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.event-card{
  padding: 20px;
  width: 250px;
  cursor: pointer;
  border: 1px solid rgb(24, 156, 117);
  margin-bottom: 18px;
}
.event-card:hover{
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgb(4, 4, 41);
}
</style>
