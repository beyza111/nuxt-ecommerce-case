<template>
  <div>
    <AppHeader />
    
    <NuxtPage />
    
    <AppFooter />
  </div>
</template>

<style>
body {
  font-family: 'Segoe UI', sans-serif;
  margin: 0;
  padding: 0;
  background-color: #fff;
}
.container {
  padding: 20px;
  max-width: 1200px;
  margin: 0 auto;
}
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); 
  gap: 40px;
}
</style>