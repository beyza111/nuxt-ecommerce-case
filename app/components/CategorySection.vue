<template>
  <section class="category-section">
    <div class="container">
      <h2 class="section-title">Featured categories</h2>
      
      <div class="category-grid">
        <div class="category-card">
          <img src="https://images.unsplash.com/photo-1585232569444-62e34bfd588d?auto=format&fit=crop&w=500&q=80" alt="Personal Care" class="bg-img">
          <div class="content-box">
            <h3>Personal Care</h3>
            <p>Lorem ipsum dolor sit amet</p>
            <button class="browse-btn">BROWSE</button>
          </div>
        </div>

        <div class="category-card">
          <img src="https://images.unsplash.com/photo-1570172619644-dfd03ed5d881?auto=format&fit=crop&w=500&q=80" alt="Skin Care" class="bg-img">
          <div class="content-box">
            <h3>Skin Care</h3>
            <p>Consectetu elit aliquam</p>
            <button class="browse-btn">BROWSE</button>
          </div>
        </div>

        <div class="category-card">
          <img src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?auto=format&fit=crop&w=500&q=80" alt="Make-Up" class="bg-img">
          <div class="content-box">
            <h3>Make - Up</h3>
            <p>Lorem ipsum dolor sit amet</p>
            <button class="browse-btn">BROWSE</button>
          </div>
        </div>

        <div class="category-card">
          <img src="https://images.unsplash.com/photo-1519689680058-324335c77eba?auto=format&fit=crop&w=500&q=80" alt="Mother & Baby" class="bg-img">
          <div class="content-box">
            <h3>Mother & Baby</h3>
            <p>Consectetu elit aliquam</p>
            <button class="browse-btn">BROWSE</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>

.category-section {
  padding: 40px 0;
  background-color: #fff;
}

.section-title {
  text-align: center;
  color: #4aa1a8;
  margin-bottom: 30px;
  font-size: 1.5rem;
}

.category-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

@media (max-width: 768px) {
  .category-grid {
    grid-template-columns: 1fr;
  }
}

.category-card {
  position: relative;
  height: 300px;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #f0f0f0; 
}

.bg-img {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0.9; 
  transition: transform 0.5s;
}

.category-card:hover .bg-img {
  transform: scale(1.1);
}

.content-box {
  position: relative;
  background: rgba(255, 255, 255, 0.95);
  padding: 20px;
  text-align: center;
  width: 50%;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.content-box h3 {
  margin: 0 0 10px 0;
  color: #333;
  font-size: 1.2rem;
}

.content-box p {
  font-size: 0.8rem;
  color: #777;
  margin-bottom: 15px;
}

.browse-btn {
  background-color: #008080; 
  color: white;
  border: none;
  padding: 8px 20px;
  font-weight: bold;
  cursor: pointer;
  transition: background 0.3s;
}

.browse-btn:hover {
  background-color: #005555;
}
</style>