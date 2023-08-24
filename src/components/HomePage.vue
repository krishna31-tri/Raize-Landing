<template>
  <div class="home">
    <div class="homepage">
      <div class="heading">
        <h1 class="headingpre">Become an investor</h1>
        <h1 class="headingpost">of the future</h1>
        <p>Access curated investments in</p>
        <span>crypto, Web3 and more</span>
      </div>
      <div class="buttons">
        <button class="genesisbutton">Become a genesis partner.</button>
        <button class="pitchbutton">Pitch Deck</button>
      </div>
      <!-- <img alt="Vue logo" src="../assets/backgroundhome.png" /> -->
    </div>
    <div class="videoside">
        <div class="video-container">
    <video controls>
      <source src="your-video-source.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "HomePage",
};
</script>
<style>
.home {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.homepage {
  display: flex;
  flex-direction: column;
}
.heading {
  display: flex;
  font-size: 30px;
  margin-left: 30px;
  flex-direction: column;
  align-items: baseline;
  padding: 30px;
}
.heading p {
  color: rgba(110, 116, 128, 1);
}
.heading span {
  margin-top: -30px;
  color: rgb(104, 104, 108);
}
.headingpost {
  margin-top: -45px;
  margin-left: -250px;
  background: linear-gradient(
    to right,
    rgb(15, 66, 233),
    rgb(160, 203, 235, 1)
  );
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
}
.buttons {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}
.genesisbutton {
  border: none;
  color: white;
  background: linear-gradient(180deg, #234ccf 0%, #4a71f0 100%, #00b4d7 100%);
  height: 70px;
  width: 309px;
  font-size: 15px;
  border-radius: 60px;
  padding: 24px 36px 24px 36px;
  top: 551px;
  gap: 12px;
  left: 100px;
}
.pitchbutton {
  color: #4a71f0;
  height: 70px;
  width: 164px;
  border-radius: 60px;
  padding: 23px 36px 23px 36px;
  background: none;
  border: 2px solid #4a71f0;
}
.videoside {
  width: 582.93px;
  height: 918.16px;
  background: url(../assets/backgroundhome.png);
}
.video-container {
    position: absolute;
    top: 50%;
    left: 66%;
    transform: translate(-50%, -50%);
    width: 86%;
    /* height: 422px; */
    max-width: 802px;
  }
</style>