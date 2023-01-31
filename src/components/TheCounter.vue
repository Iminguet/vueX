<template>
  <base-container title="Vuex">
    <h3>{{ $store.state.counter }}</h3>
  </base-container>
</template>

<script>
export default {
  computed: {
    counter() {
      return this.$store.commit('increment');
    },
  },
};
</script>
