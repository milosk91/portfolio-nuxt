<template>
  <div>
    <AboutMePage />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import AboutMePage from '~/components/AboutMePage.vue'

@Component({
  components: {
    AboutMePage,
  },
})
export default class about extends Vue {
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
