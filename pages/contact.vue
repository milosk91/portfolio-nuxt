<template>
  <div>
    <ContactMePage />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import ContactMePage from '~/components/ContactMePage.vue'

@Component({
  components: {
    ContactMePage,
  },
})
export default class contact extends Vue {
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
