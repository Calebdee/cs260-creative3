<template>
  <div>
    <PokemonView :pokemon="pokemon"/>
  </div>
</template>

<script>
// @ is an alias to /src
import PokemonView from '@/components/PokemonView.vue'
export default {
  name: 'Home',
  components: {
    PokemonView
  },
  computed: {
    pokemon() {
      return this.$root.$data.pokemon;
    }
  }
}
</script>

<style scoped>
 
</style>
