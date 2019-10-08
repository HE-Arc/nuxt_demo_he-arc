<template>
  <section class="section">
    <h1 class="title">{{ title }}</h1>
    <div class="news">
      <slot></slot>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'Section',
    props: {
      title: { type: String, }
    }

  }
</script>

<style lang="scss" scoped>

  
  .news {
    margin-left: 120px;
    margin-right: 120px;
  }
  

</style>
