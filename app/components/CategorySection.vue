<template>
  <section class="category-section">
    <div class="container">
      <h2 class="section-title">Featured Categories</h2>
      
      <div class="category-grid">
        
        <div class="category-card">
          <img src="https://manekancor.com/wp-content/uploads/2024/11/Personal-Blog-Main.jpg" alt="Personal Care" class="bg-img">
          <div class="content-box">
            <h3>Personal Care</h3>
            <p>Hair, Bath & Body</p>
            <button class="browse-btn">BROWSE</button>
          </div>
        </div>

        <div class="category-card">
          <img src="https://images.unsplash.com/photo-1570172619644-dfd03ed5d881?auto=format&fit=crop&w=500&q=80" alt="Skin Care" class="bg-img">
          <div class="content-box">
            <h3>Skin Care</h3>
            <p>Face & Treatments</p>
            <button class="browse-btn">BROWSE</button>
          </div>
        </div>

        <div class="category-card">
          <img src="https://cdn.prod.website-files.com/67336b2139b6b0905c503a6b/67a374a2cd52ad9ee0dc0f60_best-makeup-trends-and-ideas.jpeg" alt="Make-Up" class="bg-img">
          <div class="content-box">
            <h3>Make - Up</h3>
            <p>Eyes, Lips & Face</p>
            <button class="browse-btn">BROWSE</button>
          </div>
        </div>

        <div class="category-card">
          <img src="https://images.unsplash.com/photo-1519689680058-324335c77eba?auto=format&fit=crop&w=500&q=80" alt="Mother & Baby" class="bg-img">
          <div class="content-box">
            <h3>Mother & Baby</h3>
            <p>Care for Mom & Baby</p>
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
  font-weight: 600;
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
  transition: transform 0.5s;
}

.category-card:hover .bg-img {
  transform: scale(1.1);
}

.content-box {
  position: relative;
  background: rgba(255, 255, 255, 0.15);
  backdrop-filter: blur(10px); 
  -webkit-backdrop-filter: blur(10px);
  
  padding: 20px;
  text-align: center;
  width: 60%;
  
  border-radius: 0px; 
  
  box-shadow: 0 5px 15px rgba(0,0,0,0.05);
  border: 1px solid rgba(255, 255, 255, 0.2);
}

.content-box h3 {
  margin: 0 0 5px 0;
  color: #111;
  font-size: 1.2rem;
  font-weight: 600; 
  text-shadow: 0 1px 2px rgba(255,255,255,0.5);
}

.content-box p {
  font-size: 0.85rem;
  color: #222;
  margin-bottom: 15px;
  font-weight: 400; 
}

.browse-btn {
  background-color: #008080; 
  color: white;
  border: none;
  padding: 8px 25px;
  font-weight: bold;
  cursor: pointer;
  transition: background 0.3s;
  border-radius: 0px; 
}

.browse-btn:hover {
  background-color: #005555;
}
</style>