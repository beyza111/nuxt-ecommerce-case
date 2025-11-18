<template>
  <section class="promo-container">
    <div class="container promo-content">
      <div class="promo-text">
        <span class="small-tag">YOUR FAVORITES PRODUCTS</span>
        <h2>ONE CLICK AWAY FROM YOUR HOMES!</h2>
        <div class="discount-badge">
          <span class="huge-text">60%</span>
          <span class="sub-text">DISCOUNT</span>
        </div>
        <button class="shop-btn">SHOP NOW</button>
      </div>
      
     <img src="https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&w=500&q=80" alt="Cosmetic Products" class="promo-img">
    </div>
  </section>
</template>

<style scoped>
.promo-container {
  background-color: #8FD3D3; 
  margin: 40px 0;
  padding: 40px 0;
  overflow: hidden;
}

.promo-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap; 
}

.promo-text {
  color: #1a4f6d; 
  flex: 1;
  min-width: 300px;
  padding: 20px;
}

.small-tag {
  font-size: 0.9rem;
  font-weight: 600;
  letter-spacing: 1px;
}

h2 {
  font-size: 2rem;
  margin: 10px 0 20px;
}

.discount-badge {
  display: inline-block;
  margin-bottom: 20px;
  line-height: 1;
}

.huge-text {
  display: block;
  font-size: 4rem;
  font-weight: 900;
}

.shop-btn {
  background-color: #1a4f6d;
  color: white;
  padding: 10px 25px;
  border: none;
  font-weight: bold;
  cursor: pointer;
}

.promo-img {
  max-height: 300px;
  object-fit: contain;
  transform: rotate(-5deg); 
}
</style>