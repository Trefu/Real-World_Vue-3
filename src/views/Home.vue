<template>
  <h1>Events for good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'

export default {
  name: 'Home',
  components: {
    EventCard
  },
  data() {
    return {
      events: [
        {
          id: 130139,
          category: 'animal welfare',
          title: 'cat day',
          description: 'lorem impusn',
          location: 'meow town',
          date: 'Juanary 2022',
          time: '12:00',
          petsAllowed: true,
          organizer: 'kat layden'
        },
        {
          id: 9088,
          category: 'animal ionoij',
          title: 'cat month',
          description: 'lorem impusn',
          location: 'meow momomo',
          date: 'Enero 1998',
          time: '17:00',
          petsAllowed: false,
          organizer: 'kat layden'
        },
        {
          id: 89898,
          category: 'lkjkljklj welfare',
          title: 'dog day',
          description: 'lorem impusn',
          location: 'meow town',
          date: 'Febrero 2022',
          time: '9:00',
          petsAllowed: true,
          organizer: 'kjklj jkjkj'
        }
      ]
    }
  }
}
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
