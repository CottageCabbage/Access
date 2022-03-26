<template>
  <aside>
    {{cities}}
    <Checkbox name="city" value="Chicago" v-model="cities" />
    <Checkbox name="city" value="Los Angeles" v-model="cities" />
    <Checkbox name="city" value="New York" v-model="cities" />
    <Checkbox name="city" value="San Francisco" v-model="cities" />
  </aside>
</template>
<script>
import Checkbox from 'primevue/checkbox';

export default {
  components: {
    Checkbox
  },
  data () {
    return {
      cities: []
    }
  }
}
</script>

<style>
aside {
  width: 200px;
  height: 100%;
  background: #e6e6e6;
}
</style>
