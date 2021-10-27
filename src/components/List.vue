<template>
  <div v-if="toggleList">
    <h3>My list</h3>
    <ul>
      <li>item1</li>
      <li>item2</li>
      <li>item3</li>
      <li>item4</li>
    </ul>
  </div>
    <button @click="toggleListMethod">Toggle list</button>
</template>

<script>
export default {
  data() {
    return {

      toggleList: true
    }
  },
  methods: {
    toggleListMethod() {
      this.toggleList = !this.toggleList
    }
  }

}
</script>

<style>
  ul {
    display: inline;
  }
</style>