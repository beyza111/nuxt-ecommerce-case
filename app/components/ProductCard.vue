<template>
    <div class="card">
        <img :src="product.thumbnail" :alt="product.title" class="card-image" />
        
        <div class="card-details">
            <h3 class="card-title">{{ product.title }}</h3>
        
         <div class="card-footer">
            <span class="price">${{ product.price }}</span>
            <button class="add-btn">Add to Cart</button>
         </div>
        </div>
    </div>
</template>
<script setup>
defineProps(['product']);
</script>

<style scoped>
.card{

    border: 1px solid #eee;
    border-radius:8px;
    overflow: hidden;
    transition: transform 0.2s;
    background: white;
    display: flex;
    flex-direction: column;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}
 .card-image {
    width: 100%;
    height: 200px;
    object-fit: cover;
 }
 .card-details{
    padding: 15px;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
     justify-content: space-between;
}
.card-title {
  font-size: 1.1rem;
  margin: 0 0 10px 0;
  color: #333;
}

.card-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: auto; 
}

.price {
  font-weight: bold;
  font-size: 1.2rem;
  color: #2c3e50;
}

.add-btn {
  background-color: #42b883;
  color: white;
  border: none;
  padding: 8px 16px;
  border-radius: 4px;
  cursor: pointer;
  font-weight: bold;
}

.add-btn:hover {
  background-color: #3aa876;
}


</style>