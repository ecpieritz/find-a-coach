<template>
  <div>
    <section>
      FILTER
    </section>
    <section>
      <base-card>
        <div class="constrols">
          <base-button mode="outline">Refresh</base-button>
          <base-button link to="/register">Register as Coach</base-button>
        </div>
        <!-- <ul  v-if="hasCoaches"> -->
        <ul>
          <coach-item v-for="coach in filteredCoaches" :key="coach.id" :id="coach.id" :first-name="coach.firstName"
            :last-name="coach.lastName" :rate="coach.hourlyRate" :areas="coach.areas"></coach-item>
        </ul>
        <!-- <h3 v-else>No coaches found.</h3> -->
      </base-card>
    </section>
  </div>
</template>

<script>
import CoachItem from '../../components/coaches/CoachItem.vue'
import BaseCard from '../../components/ui/BaseCard.vue'
export default {
  components: {
    CoachItem,
    BaseCard
  },
  computed: {
    filteredCoaches(){
      return this.$store.getters['coaches/coaches']
    },
    hasCoaches(){
      return this.$store.getters['coaches/hasCoaches']
    }
  }
}
</script>

<style>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.controls {
  display: flex;
  justify-content: space-between;
}
</style>