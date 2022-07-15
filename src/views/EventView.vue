<script> 
import EventCard from '../components/EventCard.vue';

export default {


mounted() {
  console.log(`the component is now mounted.`, this.$route)
}

}
</script>


<template>
  <div class="about">
    <h1>Event</h1>
    <div>{{ $route.query.page}}</div>
    <div>{{ $route.params.page}}</div>
    <EventCard></EventCard>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
