<template>
  <div>
    <h1>{{ title }}</h1>
    <button @click="iAmClicked()">Click me!</button>
  </div>
</template>

<script>
var a = 0
export default {
  data() {
    return {title: 'Not clicked yet'}
  },
  methods: {
    iAmClicked() {
      this.title = 'Clicked ' + ++a + ' times';
    }
  }
};
</script>
