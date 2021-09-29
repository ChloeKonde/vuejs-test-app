<template>
  <v-app>
    <v-main>
      <TagsComponent v-bind:tags="chips" justify="start"/>
      <TagsComponent v-bind:tags="chips" justify="center"/>
    </v-main>
  </v-app>
</template>

<script>
import TagsComponent from './components/TagsComponent.vue';

export default {
  name: 'App',

  components: {
    TagsComponent,
  },

  data() {
    return {
      chips: [
        {title: "first", icon:"mdi-fire"},
        {title: "second", icon:"mdi-food-apple"},
        {title: "third", icon:"mdi-fish"},
        {title: "fourth", icon:"mdi-eye"},
        {title: "fifth", icon:"mdi-donkey"},
        {title: "sixth", icon:"mdi-dna"},
        {title: "seventh", icon:"mdi-dna"},
      ]
    }
  },
};
</script>