<template>
  <header class="site-header">
    <div class="header-content">
      <div class="logo">
        NuxtStore
      </div>
      
      <nav class="nav-links">
        <a href="#">Home</a>
        <a href="#">Products</a>
      </nav>
    </div>
  </header>
</template>

<script setup>
// No logic needed for header yet
</script>

<style scoped>
.site-header {
  background-color: #333; 
  color: white;
  padding: 1rem 0;
}

.header-content {

  max-width: 1200px; 
  margin: 0 auto;
  padding: 0 20px;
  
 
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-links a {
  color: white;
  text-decoration: none;
  margin-left: 20px;
}

.nav-links a:hover {
  color: #42b883; 
}
</style>