<template>
  <div>
    <HeroSection />
    
    <CampaignSplit />

    <div class="container">
      <h1 class="section-title">Featured Products</h1>
      <div v-if="pending" class="loading">Loading...</div>
      <div v-else class="product-grid">
        <ProductCard 
          v-for="item in data?.products" 
          :key="item.id" 
          :product="item" 
        />
      </div>
    </div>

    <PromoBanner />
    
    <CategorySection />

  </div>
</template>

<script setup>
// Veri çekme işlemi artık burada yapılacak
const { data, pending } = await useFetch('https://dummyjson.com/products?limit=8') 
</script>

<style>
/* Buraya özel stil gerekmiyor, globalden alıyor */
.section-title {
  text-align: center;
  color: #4aa1a8;
  margin: 40px 0;
}
</style>