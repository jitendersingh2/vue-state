<template>
  <div class="stats">
    <h1>A different component</h1>
    <p>There are currently {{ countLinks }} links</p>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Stats',
  computed: {
    ...mapGetters([
      'countLinks'
    ]),
  }
}
</script>