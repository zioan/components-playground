<template>
  <div class="card">
    <h2>test</h2>
    <h3>another heading</h3>
    <p v-show="showParagraph">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Culpa, voluptas!</p>
    <Button @click="toggleParagraph" :showParagraph= "showParagraph" :myData="myData"/>
    <List v-if="showParagraph"/>
  </div>
</template>

<script>
import Button from "./Button"
import List from "./List"
export default {
  data() {
    return {
      showParagraph: false,
      myData: "random text",
      

    }
  },
  components: {
    Button,
    List
  },
  methods: {
    toggleParagraph() {
      this.showParagraph = !this.showParagraph
    },
  }


}
</script>

<style>

</style>