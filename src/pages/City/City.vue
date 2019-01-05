<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
    <city-list></city-list>
    <alphabet></alphabet>
  </div>
</template>

<script type='text/ecmascript-6'>
import citySearch from './components/Search'
import cityHeader from './components/Header'
import cityList from './components/List'
import alphabet from './components/Alphabet'
export default {
  name: 'city',
  components: {
    cityHeader,
    citySearch,
    cityList,
    alphabet
  }
}
</script>

<style lang="stylus" scoped>

</style>
