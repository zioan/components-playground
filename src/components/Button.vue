<template>
<div>
  <button @click="fireAction">{{this.showParagraph}}</button>
  <p v-if="showParagraph">{{this.myData}}</p>
</div>
</template>

<script>
export default {
  props: ["showParagraph", "myData"],
  methods: {
    fireAction () {
      console.log(this.showParagraph)
      console.log(this.myData)
    }
  },


}
</script>

<style>

</style>