<template lang="html">
  <div>
    <h1>All countries</h1>
    <list-item v-for="(country, index) in countriesprop" :key="index" :countryprop="country"></list-item>
    <!-- <select> -->
      <!-- <option  v-for="(country, index) in countriesprop" :key="index" :countryprop="country" value="country"> {{country.name}} -->
      <!-- </option> -->
    <!-- </select> -->
  </div>
</template>

<script>
import ListItem from './ListItem.vue';

export default {
  name: 'countries-list',
  props: ['countriesprop'],
  components: {
    "list-item": ListItem
  }
}
</script>

<style lang="css" scoped>
</style>
