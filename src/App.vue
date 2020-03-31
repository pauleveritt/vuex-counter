<template>
  <div id="app">
    <h1>Vuex Counter</h1>
    <Counter/>
  </div>
</template>

<script>
  import Counter from './components/Counter.vue'

  export default {
    name: 'app',
    components: {
      Counter
    }
  }
</script>
