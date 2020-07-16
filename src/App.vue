<template>
  <div id="app">
    <LocaleSwitcher />
    <p>{{ $t('main.welcome', { company: 'Lokalise'}) }}</p>
  </div>
</template>

<script>
import LocaleSwitcher from './components/LocaleSwitcher'
export default {
  name: 'App',
  components: {
    LocaleSwitcher
  }
}
</script>

<style>
#app {

}
</style>
