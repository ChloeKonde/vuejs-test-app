<template>
  <v-app>
    <v-main>
      <Tags v-bind:tags="chips" justify="start"/>
      <Tags v-bind:tags="chips" justify="center"/>
    </v-main>
  </v-app>
</template>

<script>
import Tags from './components/Tags.vue';

export default {
  name: 'App',

  components: {
    Tags,
  },

  data() {
    return {
      chips: [
        {title: "Фриландские ворота", icon:" mdi-star-outline"},
        {title: "second", icon:"mdi-food-apple"},
        {title: "third", icon:"mdi-fish"},
        {title: "fourth", icon:"mdi-eye"},
        {title: "fifth", icon:"mdi-donkey"},
        {title: "sixth", icon:"mdi-fire"},
        {title: "seventh", icon:"mdi-dna"},
      ]
    }
  },
};
</script>