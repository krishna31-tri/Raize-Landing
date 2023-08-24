<template>
  <div class="compliant-main">
    <h2 class="main-heading">Compliant by design</h2>
    <P>Short description goes here</P>
    <img class="compliantbg" alt="Vue logo" src="../assets/backgroundhome.png" />
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
          <a href="https://www.finma.ch/en/authorisation/self-regulatory-organisations-sros/"
            target="_blank">self-regulatory organization (SRO)</a> according to the Anti-Money
          Laundering Act by <a
            href="https://www.finma.ch/en/authorisation/self-regulatory-organisations-sros/sro-member-search/"
            target="_blank">FINMA</a>, the Swiss financial market supervisory
          authority
        </p>
      </div>
    </div>
  </div>
</template>
<style scoped>
.compliant-main {
  width: 100vw;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 4%;
  margin-bottom: 4%;
  position: relative;
}

.main-heading {
  font-family: 'Plus Jakarta Sans';
  font-size: 36px;
  width: fit-content;
}

.compliant-flag {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  width: 100%;
  max-width: 1500px;
  margin: auto;
  padding: 1% 0% 3% 0%;
}

.compliantbg {
  position: absolute;
  top: 0%;
  left: 0%;
  width: 51%;
  height: 100%;
  z-index: -1;
}

.flag-part {
  height: 100%;
  width: 50%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.para-part {
  height: 100%;
  width: 50%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}

.para-part h3 {
  font-family: 'Plus Jakarta Sans';
  font-size: 24px;
}

.para-part p {
  font-family: 'Plus Jakarta Sans';
  font-size: 16px;
  text-align: left;
  width: 80%;
}
</style>