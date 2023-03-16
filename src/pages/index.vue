<template>
  <div>
    <button @click="countUp">Count UP</button>
    <p>{{ count }}</p>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component
export default class Index extends Vue {
  public count = 0
  public countUp() {
    this.count++
  }
}
</script>
<style scoped></style>
