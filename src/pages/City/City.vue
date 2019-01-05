<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
  </div>
</template>

<script type='text/ecmascript-6'>
import citySearch from './components/Search'
import cityHeader from './components/Header'
export default {
  name: 'city',
  components: {
    cityHeader,
    citySearch
  }
}
</script>

<style lang="stylus" scoped>

</style>
