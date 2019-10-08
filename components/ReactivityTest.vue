<template>
<div>
  <p>Name</p>
  <input type="text" v-model="textInput">
  <br>
  {{ textInput.toUpperCase() }}
  
</div>
</template>

<script>
  export default {
    name: 'ReactivityTest',
    data: () => ({
      textInput: "J'aime le cochon"
    }),
    mounted() {
    
    }

  }
</script>

<style lang="scss" scoped>

</style>
