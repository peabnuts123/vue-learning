<template>
  <transition name="slide-from-right">
    <div class="about">
      <h1>This is an about page</h1>
    </div>
  </transition>
</template>

<script lang="ts">
  import { Component, Vue } from "vue-property-decorator";

  @Component
  export default class About extends Vue {
  }
</script>
