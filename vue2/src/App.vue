<template>
  <div id="app">
    <current-timestamp></current-timestamp>
  </div>
</template>

<script>
import CurrentTimestamp from './components/CurrentTimestamp';

export default {
  name: 'App',
  components: {
    CurrentTimestamp,
  }
}
</script>