<template>
  <div>
    <HomePage />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import HomePage from '~/components/HomePage.vue'

@Component({
  components: {
    HomePage,
  },
})
export default class home extends Vue {
  /* Props */
  /* State */
  /* Data */
  /* Hooks */
  /* Methods */
  /* Computed */
  /* Watchers */
}
</script>

<style scoped>
body {
  display: flex;
  justify-content: center;
  align-items: center;
  /* background: #ececec; */
}
</style>
