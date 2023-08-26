<template>
  <div class="subscription-app">
    <h1>BECOME ONE OF OUR 200 GENESiS PARTNERS</h1>
    <table class="properties">
      <tbody>
        <tr>
          <td class="plan-details">
          </td>
          <td class="plan-details">
            <h2 style="font-size: 16px;">Basic</h2>
            <p class="free-text">Free<span class="lifetime-text">/Lifetime</span></p>
            <p style="font-size: 12px; font-weight: 500; color: rgba(145,145,163,1);">Free of charge. Start Anytime</p>
            <button class="signUp-button">Sign Up</button>
          </td>
          <td class="plan-details">
            <h2 style="font-size: 16px;">Genesis</h2>
            <p class="free-text">$500<span class="lifetime-text">/ Lifetime</span></p>
            <p style="font-size: 12px; font-weight: 500; color: rgba(145,145,163,1);">One single payment. No more!</p>
            <button class="subscribe-button">Subscribe</button>
          </td>
        </tr>
        <tr class="property-row">
          <td>Platform Fee</td>
          <td>20%</td>
          <td>10%</td>
        </tr>
        <tr class="property-row">
          <td>Referral Award</td>
          <td>0%</td>
          <td>0%</td>
        </tr>
        <tr class="property-row">
          <td>1st Level</td>
          <td>5%</td>
          <td>20%</td>
        </tr>
        <tr class="property-row">
          <td>2nd Level</td>
          <td>_</td>
          <td>10%</td>
        </tr>
        <tr class="property-row">
          <td>3rd Level</td>
          <td>_</td>
          <td>5%</td>
        </tr>
        <tr class="property-row">
          <td>OTC Deals</td>
          <td>_</td>
          <td>_</td>
        </tr>
        <tr class="property-row">
          <td>Investment Priority</td>
          <td>Lottery</td>
          <td>FCFS</td>
        </tr>
        <tr class="property-row">
          <td>Private Deals</td>
          <td>_</td>
          <td>_</td>
        </tr>
        <tr class="property-row">
          <td>Equity Deals</td>
          <td>_</td>
          <td>_</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {

};
</script>

<style>
.free-text {
  font-size: 40px;
  font-family: 'Plus Jakarta Sans';
  color: rgba(74, 113, 240, 1);

}

.lifetime-text {
  font-size: 16px;
  font-family: 'Plus Jakarta Sans';
  color: rgba(74, 113, 240, 1);

}

.subscribe-button {
  height: 42px;
  width: 342px;
  border-radius: 60px;
  border: 1px;
  background: rgba(74, 113, 240, 1);
  color: white;
}

.subscription-app {
  font-family: Arial, sans-serif;
  margin: 20px;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th,
td {
  padding: 10px;
  text-align: center;
}

th {
  background-color: #f0f0f0;
}

.plan-header {
  background-color: rgba(240, 245, 250, 1);
}

.plan-details {
  background-color: white;
}

.property-row:nth-child(even) {
  background-color: rgba(240, 245, 250, 1);
}

.property-row:nth-child(odd) {
  background-color: white;
}

h2 {
  margin: 5px 0;
}

.subscription td {
  border: none;
  padding: 0;
}

.subscription h2 {
  text-align: center;
}

.subscription p {
  text-align: center;
  margin: 5px 0;
}

.subscription button {
  display: block;
  margin: 0 auto;
}

.signUp-button {
  height: 42px;
  width: 342px;
  border-radius: 60px;
  border: 1px;
  background: linear-gradient(0deg, #DAE2FA, #DAE2FA), linear-gradient(0deg, #FFFFFF, #FFFFFF);
  color: rgba(0, 29, 61, 1);
}

@media (max-width:768px) {
  .subscription-app {
    display: none;
  }
}
</style>