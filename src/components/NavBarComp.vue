
<template>
  <nav class="navbar navbar-expand-lg navBar">
    <div class="container-fluid">
      <a class="navbar-brand nav-link" href="../index.html">XCLUSIVECLEETS</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav ms-auto">
          <router-link  class="nav-link" to="/">HOME</router-link>
          <router-link  class="nav-link" to="/about">ABOUT</router-link>
          <router-link  class="nav-link" to="/products">PRODUCTS</router-link>
          <router-link  class="nav-link" to="/admin">ADMIN</router-link>
          <router-link  class="nav-link" to="/checkout">CHECKOUT</router-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

</style>