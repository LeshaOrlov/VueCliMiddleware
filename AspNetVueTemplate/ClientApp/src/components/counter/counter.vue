﻿<template>
  <div>
    <h1>Counter</h1>

    <p>This is a simple example of a Vue.js component.</p>

    <p>
      Current count: <strong>{{ currentcount }}</strong>
    </p>

    <v-btn @click="incrementCounter">Increment</v-btn>
  </div>
</template>

<script>
export default {
  name: "counter",
  data() {
    return {
      currentcount: 0,
    };
  },
  methods: {
    incrementCounter() {
      this.currentcount++;
    },
  },
};
</script>