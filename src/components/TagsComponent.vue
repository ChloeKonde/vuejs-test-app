<template>
<v-container>
 <v-row :justify="justify">
    <v-col
      cols="2"
      sm="1"
      md="6"
      lg="5">

        <div>
          <v-chip-group
            column>

            <v-chip outlined
              v-for="tag in tags"
              :key="tag">
              
              <v-icon left>
                {{ tag.icon }}
              </v-icon>

              {{ tag.title }}
              
            </v-chip>

            
          </v-chip-group>
        </div>
    </v-col>
  </v-row>
</v-container>
</template>

<style scoped>
</style>

<script>
  export default {
    name: 'TagsComponent',
    props: ['tags', 'justify']
    }
</script>
