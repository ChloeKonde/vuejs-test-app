<template>
<div class="chip-group-wrapper">
<v-container>
 <v-row :justify="justify">
    <v-col
      cols="2"
      sm="7"
      md="6"
      lg="5">

          <v-chip-group class="chip-group-wrapper__group"
            column>

            <v-chip 
              class="chip-group-wrapper__chip" outlined
              v-for="tag in tags"
              :key="tag">
              
              <v-icon left>
                {{ tag.icon }}
              </v-icon>

              {{ tag.title }}
              
            </v-chip>

            
          </v-chip-group>
    </v-col>
  </v-row>
</v-container>
</div>

</template>

<style lang="scss">
@import "@/sass/variables.scss";

.chip-group-wrapper__chip {
  font-family: $mulish;
}
</style>

<script>
  export default {
    name: 'Tags',
    props: ['tags', 'justify']
    }
</script>
