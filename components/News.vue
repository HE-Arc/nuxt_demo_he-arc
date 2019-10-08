<template>
  <div class="wrapper">
    <span class="news-title">{{ news.title }}</span>
    <span class="body">{{ news.body }}</span>
  </div>
</template>

<script>
  export default {
    props: {
      news: { type: Object }
    },
    name: 'News'
  }
</script>

<style lang="scss" scoped>
  
  .wrapper {
    display: flex;
    flex-direction: column;
    border: 1px solid gray;
    margin-bottom: 20px;
    padding: 10px;
    border-radius: 10px;
    
    
    
    .news-title {
      font-weight: bold;
      font-size: 32px;
      color: gray;
      padding-bottom: 10px;
    }
  
    .body {
    
    }
  }
  

</style>
