<template>
  <div>
    <ProjectsPage />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import ProjectsPage from '~/components/ProjectsPage.vue'

@Component({
  components: {
    ProjectsPage,
  },
})
export default class projects extends Vue {
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
