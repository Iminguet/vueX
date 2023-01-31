<template>
  <base-container title="Vuex">
    <h3>{{ $store.state.counter }}</h3>

    <button @click="addOne">Add 1</button>
  </base-container>
</template>

<script>
export default {
  computed: {
    counter() {
      return this.$store.state.counter;
    },
  },
};
</script>
