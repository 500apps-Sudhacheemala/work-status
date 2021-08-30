<template>
<desktop></desktop>
<document></document>
<downloads></downloads>


</template>

<script>
import desktop from './components/desktop.vue'
import document from './components/document.vue'
import downloads from './components/downloads.vue'


export default {
  name: 'App',
  components: {
    desktop,
    document,
    downloads,
  }
}
</script>

<style>

</style>
