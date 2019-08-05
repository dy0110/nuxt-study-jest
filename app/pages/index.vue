<template>
  <div>
    <h2>カウンター</h2>
    <h3>Count: {{}}</h3>
    <button type="button" @click="increment"></button>
  </div>
</template>

<script>
import { mapGetters, mapActions } from "vuex";

export default {
  computed: {
    ...mapGetters(["count"])
  },
  methods: {
    ...mapActions(["increment"])
  }
};
</script>
