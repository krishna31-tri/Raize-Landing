<template>
  <div>
    <div class="footer">
      <div class="footer-item">
        <h1>More Information</h1>
        <p>FAQ</p>
        <p>Deck</p>
        <p>Support</p>
        <p>Media Deck</p>
        <p>Press Inquiries</p>
        <div class="copyright">
          <p>&copy; 2023 Raizers. All rights reserved.</p>
        </div>
      </div>
      <div class="footer-item">
        <h1>Legal Agreement</h1>
        <p>Terms & Conditions</p>
        <p>Partner's Incentive Agreement</p>
        <p>Privacy Policy</p>
        <p>Risk Disclaimer</p>
        <p>Cookie Policy</p>
      </div>
      <div class="footer-item">
        <h1>Web³ CROWDFUNDING PLATFORM</h1>
        <p>Subscribe to our newsletter to get updates about our services and offers</p>
        <div class="input-container">
          <input type="text" placeholder="Enter your email...." class="email-input" />
          <button class="submit-button">Subscribe</button>
        </div>
        <div class="media-icons">
          <img src="../assets/LinkedIn_icon.png" alt="LinkedIn" />
          <img src="../assets/Logo_of_Twitter.png" alt="Twitter" />
          <img src="../assets/Telegram_logo.png" alt="Telegram" />
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
  flex-wrap: wrap;
  justify-content: space-evenly;
  padding: 40px 0;
  text-align: start;

}

.footer-item {
  flex: 1;
  max-width: 300px;
  margin: 0 10px;
  color: white;
  font-size: 13px;
}

.footer-item h1 {
  font-size: 24px;
  margin-bottom: 10px;
  text-align: start;
}

.footer-item p {
  color: #c4c4c4;
  font-size: 13px;
  margin-bottom: 5px;
}

.input-container {
  margin-top: 20px;
  display: flex;
  align-items: center;
}

.email-input {
  flex: 1;
  height: 50px;
  padding: 10px;
  text-align: left;
  border: 1px solid white;
  background: none;
  border-radius: 60px;
  color: white;
}

.submit-button {
  height: 71px;
  width: 160px;
  border-radius: 60px;
  padding: 0 36px;
  margin-left: 10px;
  background-color: #4a71f0;
  border: none;
  color: white;
  margin-left: -45%;
}

.media-icons {
  margin-top: 10px;
  display: flex;
  justify-content: space-between;
  width: 100px;
}

@media (max-width: 1100px) {
  .footer-item {
    min-width: 42%;
  }

  .footer {
    background-color: #001d3d;
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    padding: 40px;
    text-align: start;
  }

  .submit-button {
    margin-left: -30%;
  }
}

@media (max-width: 768px) {
  .footer {
    flex-direction: column;
    align-items: flex-start;
    padding: 8%;
  }

  .footer-item {
    max-width: 100%;
    text-align: start;
    margin: 15px 0;
  }

  .submit-button {
    margin-left: -30%;
  }

  .media-icons {
    width: 42%;
    justify-content: space-around;
    margin: auto;
    margin-top: 7%;
  }
}
</style>
