<template lang="html">
  <div>
    <list-item v-for="(country, index) in countries" :country="country" :key="index"></list-item>
  </div>
</template>

<script>
import ListItem from './ListItem.vue';

export default {
  name: 'countries-list',
  props: ['countries'],
  components: {
    "list-item": ListItem
  }
}
</script>

<style lang="css" scoped>
</style>
