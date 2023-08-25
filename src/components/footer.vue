<template>
  <div>
    <div class="footer">
      <div class="Footer-item1">
        <h1>More Information</h1>
        <p>FAQ</p>
        <p>Deck</p>
        <p>Support</p>
        <p>Media Deck</p>
        <p>press Inquiries</p>
        <div class="copyright">
          <p>&copy; 2023 Raizers. All rights reserved.</p>
        </div>
      </div>
      <div class="Footer-item">
        <h1>Legal Agreement</h1>
        <p>Terms & Conditions</p>
        <p>Partner's Incentive Agreement</p>
        <p>Privacy Policy</p>
        <p>Risk disclaimer</p>
        <p>Cookie policy</p>
      </div>
      <div class="Footer-item">
        <h1>Web³ CROWDFUNDING PLATFORM</h1>
        <p>Subscribe to our newsletter to get updates about our services and offers</p>
        <div class="input-container">
          <input type="text" placeholder="Enter your email...." class="email-input" />
          <button class="submit-button">Subscribe</button>
        </div>
        <div class="media-icons">
          <img src="../assets/LinkedIn_icon.png" />
          <img src="../assets/Logo_of_Twitter.png" />
          <img src="../assets/Telegram_logo.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterPage",
};
</script>

<style scoped>
.footer {
  background-color: #001d3d;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: flex-start;
  flex-wrap: wrap;
  padding: 40px 0;
}

.Footer-item1 {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  color: white;
  font-size: 13px;
  margin-top: 20px;
  margin-right: 20px;
}

.Footer-item {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  color: white;
  font-size: 13px;
  margin-top: 20px;
  margin-right: 20px;
}

.Footer-item h1 {
  font-size: 24px;
  margin-bottom: 10px;
}

.Footer-item p {
  color: #c4c4c4;
  font-size: 13px;
  margin-bottom: 5px;
}

.input-container {
  position: relative;
  display: inline-block;
  margin-bottom: 20px;
}

.email-input {
  width: 460px;
  height: 50px;
  padding: 10px;
  text-align: left;
  border: 1px solid white;
  background: none;
  margin-top: 22px;
  border-radius: 60px;
}
.submit-button {
  position: absolute;
  height: 72px;
  width: 160px;
  right: 0;
  border-radius: 60px;
  padding: 24px 36px 24px 36px;
  margin-top: 22px;
  background-color: #4a71f0;
}

.media-icons {
  margin-top: 10px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100px;
}

@media (max-width: 768px) {
  .Footer-item1, .Footer-item, .Footer-item h1, .Footer-item p {
    /* font-size: 12px; */
  }
  
  .input-container {
    /* flex-direction: column;
    align-items: flex-start;
    margin-bottom: 20px; */
  }
  
  .email-input {
    /* width: 100%;
    margin-right: 0;
    margin-bottom: 5px; */
  }
  
  .submit-button {
    /* width: 100%; */
  }
  
  .media-icons {
    width: 100%;
    justify-content: flex-start;
  }
}
</style>
