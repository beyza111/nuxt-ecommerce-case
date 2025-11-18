<template>
  <div class="checkout-page">
    <div class="container">
      
      <h1 class="page-title">Checkout</h1>
      
      <div class="checkout-grid">
        
        <div class="checkout-form">
          
          <section class="form-section">
            <h2 class="section-header">
              <span class="icon">📦</span> Shipping details
            </h2>
            
            <div class="form-row">
              <div class="form-group half">
                <label>First Name *</label>
                <input type="text" />
              </div>
              <div class="form-group half">
                <label>Last Name *</label>
                <input type="text" />
              </div>
            </div>

            <div class="form-row">
              <div class="form-group half">
                <label>Email Address *</label>
                <input type="email" />
              </div>
              <div class="form-group half">
                <label>Phone Number *</label>
                <input type="text" placeholder="+1 (555) ... .. .." />
              </div>
            </div>

            <div class="form-row">
              <div class="form-group half">
                <label>City *</label>
                <select><option>Please select</option></select>
              </div>
              <div class="form-group half">
                <label>State *</label>
                <select><option>Please select</option></select>
              </div>
            </div>

            <div class="form-group full">
              <label>Address *</label>
              <textarea placeholder="Enter street address, apartment, suite, etc."></textarea>
            </div>
          </section>

          <section class="form-section">
            <h2 class="section-header">
              <span class="icon">💳</span> Payment details
            </h2>
            
            <div class="form-group full">
              <label>Card Holder Name *</label>
              <input type="text" />
            </div>
            
            <div class="card-input-wrapper">
               <div class="form-group full">
                  <label>Card Number *</label>
                  <input type="text" placeholder="0000 0000 0000 0000" />
               </div>
            </div>

            <div class="form-row">
              <div class="form-group half">
                <label>Expiry Date *</label>
                <input type="text" placeholder="MM / YY" />
              </div>
              <div class="form-group half">
                <label>CVV *</label>
                <input type="text" />
              </div>
            </div>
          </section>
          
          <button class="pay-btn">PAY NOW ($84.90)</button>

        </div>

        <div class="checkout-summary">
          <h3>Shopping cart summary</h3>
          
          <div class="summary-item">
            <img src="https://media.sephora.eu/content/dam/digital/pim/published/S/SISLEY/743628/357024-media_swatch-1.jpeg" alt="Hair Mask" />
            <div class="item-info">
              <h4>The Intense Nutrition Hair Mask</h4>
              <div class="price-row">
                <span>$44.95</span>
                <span class="qty">x 1</span>
              </div>
            </div>
          </div>

          <div class="summary-item">
            <img src="https://images.unsplash.com/photo-1631729371254-42c2892f0e6e?auto=format&fit=crop&w=200&q=80" alt="Shampoo" />
            <div class="item-info">
              <h4>Strengthening Shampoo</h4>
              <div class="price-row">
                <span>$29.45</span>
                <span class="qty">x 1</span>
              </div>
            </div>
          </div>

          <div class="discount-code">
            <input type="text" placeholder="Discount code" />
          </div>

          <div class="totals">
            <div class="row">
              <span>Subtotal</span>
              <span>$74.40</span>
            </div>
            <div class="row">
              <span>Shipping</span>
              <span>$10.50</span>
            </div>
            <div class="row total">
              <span>Total</span>
              <span>$84.90</span>
            </div>
          </div>

        </div>

      </div>
    </div>
  </div>
</template>

<style scoped>
.checkout-page {
  background-color: #f9f9f9;
  min-height: 100vh;
  padding-bottom: 50px;
}

.page-title {
  font-size: 2rem;
  margin: 20px 0 30px;
  color: #333;
}

.checkout-grid {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 40px;
}

@media (max-width: 768px) {
  .checkout-grid {
    grid-template-columns: 1fr;
  }
}

.section-header {
  font-size: 1.2rem;
  margin-bottom: 20px;
  border-bottom: 1px solid #eee;
  padding-bottom: 10px;
  display: flex;
  align-items: center;
  gap: 10px;
}

.form-row {
  display: flex;
  gap: 20px;
  margin-bottom: 20px;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.half { width: 50%; }
.full { width: 100%; }

label {
  font-size: 0.85rem;
  font-weight: 600;
  color: #555;
}

input, select, textarea {
  padding: 12px;
  border: 1px solid #ddd;
  border-radius: 4px;
  background-color: #fff;
  font-size: 0.9rem;
}

textarea {
  height: 80px;
  resize: none;
}

.pay-btn {
  background-color: #ea4c89;
  color: white;
  border: none;
  width: 100%;
  padding: 15px;
  font-weight: bold;
  font-size: 1rem;
  border-radius: 4px;
  cursor: pointer;
  margin-top: 20px;
}

.checkout-summary {
  background-color: #fff;
  padding: 20px;
  border-radius: 8px;
  height: fit-content;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}

.summary-item {
  display: flex;
  gap: 15px;
  margin-bottom: 20px;
  padding-bottom: 20px;
  border-bottom: 1px solid #eee;
}

.summary-item img {
  width: 70px;
  height: 70px;
  object-fit: cover;
  border: 1px solid #eee;
  border-radius: 4px;
}

.item-info h4 {
  font-size: 0.9rem;
  margin: 0 0 5px;
  color: #333;
}

.price-row {
  display: flex;
  justify-content: space-between;
  font-size: 0.9rem;
  color: #666;
}

.discount-code input {
  width: 100%;
  margin-bottom: 20px;
}

.totals .row {
  display: flex;
  justify-content: space-between;
  margin-bottom: 10px;
  font-size: 0.9rem;
  color: #555;
}

.totals .total {
  font-weight: 900;
  color: #000;
  font-size: 1.1rem;
  border-top: 1px solid #ddd;
  padding-top: 15px;
  margin-top: 10px;
}
</style>