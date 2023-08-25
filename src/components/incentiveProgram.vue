<template>
  <div class="incentive-program">
    <img class="incentivebg" alt="Vue logo" src="../assets/incentivebg.png" />
    <div class="incentive-program-div">
      <h1 class="heading">A Unique Partner's Incentive Program</h1>
      <div class="card-container1">
        <img class="linebg" alt="Vue logo" src="../assets/linebg.svg" />
        <div class="main-card card1">
          <div class="inner-card">
            <div class="referral-link">
              <p>My referral link...</p>
              <img src="../assets/Copyicon.png" />
            </div>
            <div class="social-media-icons">
              <a href="https://www.telegram.com" target="_blank">
                <img src="@/assets/TeleIncentive.png" alt="Telegram Icon" />
              </a>
              <a href="https://www.twitter.com" target="_blank">
                <img src="@/assets/TwitterIncentive.png" alt="Twitter Icon" />
              </a>
              <a href="https://www.gmail.com" target="_blank">
                <img src="@/assets/GmailIncentive.png" alt="mail Icon" />
              </a>
              <a href="https://www.linkedin.com" target="_blank">
                <img src="@/assets/LinkedinIncentive.png" alt="linkedin Icon" />
              </a>
              <span style="color: white; font-size: 30px">....</span>
              <!-- Add more anchor tags and img tags for additional icons as needed -->
            </div>
          </div>
          <h3 style="font-size: 24px; width: 200px">
            Share your link to your friends
          </h3>
        </div>

        <div class="card-component">
          <div class="main-card">
            <div class="inner-card1">
              <img class="tick-icon" src="../assets/TickIcon.png" />
              <button class="sign-in-button">Sign In</button>
            </div>
            <div class="background-card"></div>
          </div>
          <h3 style="font-size: 24px">Your Contact Sign in</h3>
        </div>

        <div class="main-card card1">
          <div class="inner-card">
            <img style="height: 80px; width: 80px; margin-left: 58px" src="../assets/contact-invest.png" />
          </div>
          <h3 style="font-size: 24px; width: 200px">Your contact invest</h3>
        </div>

        <div class="card-component">
          <div class="main-card">
            <div class="inner-card1">
              <h3>Unlimited Rewards</h3>
              <div class="rewards-icons">
                <img src="../assets/rewards-icon1.png" />
                <img src="../assets/rewards-icon2.png" />
                <img src="../assets/rewards-icon3.png" />
              </div>
            </div>
            <div class="background-card"></div>
          </div>
          <h3 style="font-size: 24px; width: 333px;">
            Unlimited rewards based fee taken on-chain distribute
          </h3>
        </div>
        <!-- Add more cards as needed -->
      </div>
      <button class="partner-button">Become a Partner</button>
    </div>

  </div>
</template>
  
<script>
export default {
  name: "Incentive_Program",
  methods: {
    copyToClipboard() {
      // Logic to copy referral link to clipboard
    },
  },
};
</script>
  
<style>
.card-component {
  display: flex;
  flex-direction: column;
  height: 395px;
  align-items: center;
}

.incentivebg {
  position: absolute;
  top: 0%;
  left: 0%;
  width: 97%;
  height: 100%;
  z-index: -1;
}

.incentive-program {
  text-align: center;
  padding: 20px;
  position: relative;
  padding-bottom: 7%;
  margin-top: 5%;
}

.incentive-program-div {
  width: 90%;
  max-width: 1500px;
  margin: auto;

}

.heading {
  font-size: 24px;
  margin-bottom: 20px;
}

.card-container1 {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  margin-top: 38px;
  flex-wrap: wrap;
  position: relative;
}

.linebg {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -100%);
  width: 84%;
  z-index: -1;
}

.main-card {
  width: 200px;
  height: 420px;
  position: relative;
  /* border: 1.3px solid rgba(74, 113, 240, 1); */
  /* border-radius: 6px; */
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
}

.partner-button {
  height: 70px;
  border-radius: 60px;
  width: 225px;
  border: 1px solid rgba(74, 113, 240, 1);
  background: none;
  color: rgba(74, 113, 240, 1);
  font-size: 18px;
  font-family: 'Plus Jakarta Sans';
  margin-top: 40px;
}

.sign-in-button {
  height: 48px;
  width: 153px;
  color: white;
  border-radius: 20px;
  background-color: rgba(74, 113, 240, 1);
  border: none;
}

.inner-card {
  width: 200px;
  height: 200px;
  position: relative;
  border: 1.3px solid rgba(74, 113, 240, 1);
  border-radius: 6px;
  padding: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-color: rgba(74, 113, 240, 1);
  box-shadow: 0px 10px 20px 0px rgba(74, 113, 240, 0.5);
}

.inner-card1 {
  width: 200px;
  height: 200px;
  position: absolute;
  border-radius: 6px;
  padding: 20px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 10px 20px 0px rgba(74, 113, 240, 0.5);
  align-content: center;
  align-items: center;
}

.referral-link {
  background: rgba(234, 238, 254, 1);
  padding: 5px;
  border-radius: 20px;
  height: 26.14px;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  color: rgba(74, 113, 240, 1);
}

.social-media-icons {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  margin-top: 9px;
}

.background-card {
  width: 247px;
  height: 249px;
  position: absolute;
  /* top: 141px; */
  /* left: 323.87939453125px; */
  z-index: -1;
  border-radius: 12px;
  transform: rotate(7deg);
  background: rgba(74, 113, 240, 1);
}

/* Include a link to the Font Awesome CSS for the icons */
</style>
  