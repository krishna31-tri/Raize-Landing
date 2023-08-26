<template>
  <div class="subscription-app">
    <h1>Become one of our 200 genesis partners</h1>
    <div class="properties">
      <div class="plan-details" id="pd1">
        <div class="plan-header"></div>
        <ul class="plan-header-content">
          <li>Platform fee</li>
          <li>Referral reward</li>
          <li>1st Level</li>
          <li>2nd Level</li>
          <li>3rd Level</li>
          <li>OTC Deals</li>
          <li>Investment Priority</li>
          <li>Private Deals</li>
          <li>Equity Deals</li>
        </ul>
      </div>
      <div class="plan-details">
        <div class="plan-header">
          <h2 style="font-size: 16px;">Basic</h2>
          <p class="free-text">Free<span class="lifetime-text">/Lifetime</span></p>
          <p style="font-size: 12px; font-weight: 500; color: rgba(145,145,163,1);">Free of charge. Start Anytime</p>
          <button class="signUp-button">Sign Up</button>
        </div>


        <ul class="plan-header-content">
          <li>20 %</li>
          <li></li>
          <li>5%</li>
          <li>-</li>
          <li>-</li>
          <li>-</li>
          <li>Lottery</li>
          <li>-</li>
          <li>-</li>
        </ul>
      </div>
      <div class="plan-details" id="pd3">
        <div class="exclusive">
          Exclusive
        </div>
        <div class="plan-header">
          <h2 style="font-size: 16px;">Genesis</h2>
          <p class="free-text">$500<span class="lifetime-text">/ Lifetime</span></p>
          <p style="font-size: 12px; font-weight: 500; color: rgba(145,145,163,1);">One single payment. No more!</p>
          <button class="subscribe-button">Subscribe</button>
        </div>
        <ul class="plan-header-content">
          <li>10%</li>
          <li></li>
          <li>20%</li>
          <li>10%</li>
          <li>5%</li>
          <li>✔️</li>
          <li>FCFS</li>
          <li>✔️</li>
          <li>✔️</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style>
.subscription-app {
  font-family: Arial, sans-serif;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 80%;
  max-width: 1500px;
  margin: auto;
  position: relative;
}


h1 {
  font-family: 'Plus Jakarta Sans';
  font-size: 36px;
  width: -moz-fit-content;
  width: fit-content;
  text-align: center;
}

.properties {
  display: flex;
  justify-content: space-between;
  margin-top: 20px;
}

.plan-details {
  flex: 1;
  background-color: white;
  width: 75%;
}

.plan-header {
  height: 255px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  width: 300px;
}

.subscription-app ul {
  margin: 0;
  padding: 0;
}

.subscription-app li {
  list-style: none;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}

#pd1 li {
  color: #4A71F0;
  text-align: start;
  justify-content: flex-start;
  padding-left: 25%;
}

#pd3 {
  border: 2px solid #4A71F0;
  border-radius: 8px;
  position: relative;
  z-index: 2;
}

.exclusive {
  position: absolute;
  top: -3%;
  left: 50%;
  transform: translateX(-50%);
  background-color: #DAE2FA;
  color: #4A71F0;
  padding: 2% 4%;
  border-radius: 30px;
}

.subscription-app li:nth-child(odd) {
  background-color: #F0F5FA;
}

.free-text {
  font-size: 40px;
  font-family: 'Plus Jakarta Sans';
  color: rgba(74, 113, 240, 1);
  margin: 7px;
  font-weight: 600;

}

.lifetime-text {
  font-size: 16px;
  font-family: 'Plus Jakarta Sans';
  color: rgba(74, 113, 240, 1);
}

.subscribe-button,
.signUp-button {
  border-radius: 60px;
  width: 90%;
  margin: auto;
  border: none;
  color: white;
  cursor: pointer;
  font-size: 14px;
  font-weight: bold;
  padding: 4% 0;
  transition: background-color 0.3s ease;
}

.subscribe-button {
  background: rgba(74, 113, 240, 1);
}

.signUp-button {
  background: linear-gradient(0deg, #DAE2FA, #DAE2FA), linear-gradient(0deg, #FFFFFF, #FFFFFF);
  color: rgba(0, 29, 61, 1);
}

.property-row {
  display: flex;
  justify-content: space-between;
  background-color: rgba(240, 245, 250, 1);
  padding: 10px 20px;
  margin-top: 10px;
}

.property-details {
  flex: 1;
  color: #4A71F0;
  font-weight: bold;
  text-align: center;
}

@media (max-width: 768px) {
  .subscription-app {
    display: none;
  }
}
</style>

