<template>
  <div id="app">
    <app-header/>
    <section class="container">
      <app-grid/>
    </section>
    <app-form/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppGrid from "./components/AppGrid.vue";
import AppForm from "./components/AppForm.vue";

export default {
  components: {
    AppHeader,
    AppGrid,
    AppForm
  },
  created() {
    this.$store.commit("initialArrIndex", window.location.search);
  }
};
</script>

<style lang="scss">
#app {
  margin: 1vmin 1vmin 0;
}

.container {
  display: flex;
}

@media screen and (max-width: 700px) {
  .container {
    flex-direction: column;
  }
}
</style>
