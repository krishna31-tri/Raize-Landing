<template>
  <div class="compliant-main">
    <h2 class="main-heading">Compliant by design</h2>
    <div class="compliant-flag">
      <div class="flag-part">
        <img src="../assets/swissFlag.png" />
      </div>
      <div class="para-part">
        <h3>A swiss compliant company</h3>
        <p>
          Raize Partners is a company established in Switzerland since 2023 with
          offices in Lausanne, and is an affiliated-to-be financial intermediary
          with a first-rate track record in compliance and due diligence.
        </p>
        <p>
          We are in the process of being affiliated to an officially recognized
          <a href="https://www.finma.ch/en/authorisation/self-regulatory-organisations-sros/" target="_blank">self-regulatory organization (SRO)</a> according to the Anti-Money
          Laundering Act by <a href="https://www.finma.ch/en/authorisation/self-regulatory-organisations-sros/sro-member-search/" target="_blank">FINMA</a>, the Swiss financial market supervisory
          authority
        </p>
      </div>
    </div>
  </div>
</template>
<style scoped>
.main-heading{
    font-family: 'Plus Jakarta Sans';
    font-size: 36px;
}
.compliant-flag{
    display: flex;
    flex-direction: row;
    align-content: center;
    align-items: center;
}
.flag-part{
    height: 500px;
    width: 50%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
.para-part{
    height: 500px;
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
}
.para-part h3{
    font-family: 'Plus Jakarta Sans';
    font-size: 24px;
}
.para-part p{
    font-family: 'Plus Jakarta Sans';
    font-size: 16px;
    text-align: left;
    width: 677px;
}
</style>