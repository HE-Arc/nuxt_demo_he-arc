<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="https://bulma.io">
        <p class="title">{{ title }}</p>
      </a>
  
      <a role="button"
         class="navbar-burger burger"
         aria-label="menu"
         aria-expanded="false"
         data-target="navbarBasicExample">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>
  
    <div id="navbarBasicExample" class="navbar-menu">
      
      <div class="navbar-start">
        
        <a v-for="cat in categories" class="navbar-item">
          {{ cat.title }}
        </a>
        
      </div>

    </div>
  </nav>
</template>

<script>
  export default {
    name: 'Navbar',
    props: {
      title: { type: String }
    },
    data: () => ({
      categories: [
        { title: 'information' },
        { title: 'contact' },
        { title: 'about' },
        { title: 'articles' }
      ]
    })

  }
</script>

<style lang="scss" scoped>
  .navbar {
    border-bottom: 1px solid lightgray;
  
  }
</style>
