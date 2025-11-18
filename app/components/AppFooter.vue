<template>
  <footer class="site-footer">
    
    <div class="newsletter-section">
      <div class="container newsletter-content">
        <div class="newsletter-text">
          <h3>Sign up to our newsletter</h3>
          <p>Be the first to hear about the latest offers.</p>
        </div>
        
        <div class="newsletter-form">
          <input type="email" placeholder="Your email address" />
          <button>SUBSCRIBE</button>
        </div>
      </div>
    </div>

    <div class="footer-links-section">
      <div class="container links-grid">
        
        <div class="footer-col">
          <h4>CORPORATE</h4>
          <ul>
            <li><a href="#">About Us</a></li>
            <li><a href="#">Press</a></li>
            <li><a href="#">Human Resources</a></li>
            <li><a href="#">News From Us</a></li>
          </ul>
        </div>

        <div class="footer-col">
          <h4>SHOPPING</h4>
          <ul>
            <li><a href="#">Order and Payment</a></li>
            <li><a href="#">Cancellation and Refund</a></li>
            <li><a href="#">Delivery Conditions</a></li>
            <li><a href="#">Secure Shopping</a></li>
          </ul>
        </div>

        <div class="footer-col">
          <h4>LEGAL</h4>
          <ul>
            <li><a href="#">Terms of Use</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li><a href="#">Membership Agreement</a></li>
            <li><a href="#">Distance Selling Contract</a></li>
          </ul>
        </div>

        <div class="footer-col">
          <h4>HELP CENTER</h4>
          <ul>
            <li><a href="#">FAQ</a></li>
            <li><a href="#">Contact Center</a></li>
          </ul>
        </div>

        <div class="footer-col contact-col">
          <h4>CONTACT US</h4>
          <p>Saray Mah. Site Yolu Cad. Anel İş Merkezi, Ümraniye/İstanbul</p>
          <p class="phone">0850 755 9987</p>
          <p>info@watsons.com.tr</p>
          
          <div class="social-icons">
            <span class="icon">f</span>
            <span class="icon">t</span>
            <span class="icon">in</span>
            <span class="icon">ig</span>
          </div>
        </div>

      </div>
    </div>

    <div class="copyright-bar">
      <div class="container">
        <p>&copy; 2025 WATSONS. ALL RIGHTS RESERVED.</p>
      </div>
    </div>

  </footer>
</template>

<style scoped>
.site-footer {
  background-color: #fff;
  margin-top: 50px;
}

/* Newsletter Section */
.newsletter-section {
  background-color: #f3f3f3; 
  padding: 30px 0;
  border-top: 1px solid #e0e0e0;
}

.newsletter-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 20px;
}

.newsletter-text h3 {
  margin: 0;
  font-size: 1.1rem;
  color: #333;
}

.newsletter-text p {
  margin: 5px 0 0;
  font-size: 0.85rem;
  color: #666;
}

.newsletter-form {
  display: flex;
  gap: 10px;
  flex: 1;
  max-width: 500px;
}

.newsletter-form input {
  flex: 1;
  padding: 10px 15px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

.newsletter-form button {
  background-color: #ea4c89; 
  color: white;
  border: none;
  padding: 10px 25px;
  font-weight: bold;
  border-radius: 4px;
  cursor: pointer;
}

/*Footer Links*/
.footer-links-section {
  padding: 50px 0;
  background-color: #f9f9f9;
}

.links-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 30px;
}

.footer-col h4 {
  font-size: 0.8rem;
  color: #333;
  margin-bottom: 20px;
  font-weight: bold;
}

.footer-col ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.footer-col li {
  margin-bottom: 10px;
}

.footer-col a {
  text-decoration: none;
  color: #666;
  font-size: 0.8rem;
  transition: color 0.2s;
}

.footer-col a:hover {
  color: #ea4c89;
}

.contact-col p {
  font-size: 0.8rem;
  color: #666;
  line-height: 1.5;
  margin-bottom: 10px;
}

.phone {
  font-weight: bold;
  color: #333 !important;
}

.social-icons {
  display: flex;
  gap: 10px;
  margin-top: 15px;
}

.icon {
  width: 30px;
  height: 30px;
  background-color: #ddd;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 0.8rem;
  color: white;
  font-weight: bold;
  cursor: pointer;
}

.icon:hover {
  background-color: #4aa1a8;
}

/* --- Copyright --- */
.copyright-bar {
  background-color: #eeeeee;
  padding: 15px 0;
  text-align: center;
  font-size: 0.75rem;
  color: #999;
}
</style>