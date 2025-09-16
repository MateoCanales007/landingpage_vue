<template>
  <AppContent />
  <AppFooter />
</template>

<script>
import AppFooter from './components/AppFooter.vue'
import AppContent from './components/AppContent.vue'

export default {
  name: 'App',
  components: {
    AppContent,
    AppFooter
  }
}
</script>

<style>
</style>
