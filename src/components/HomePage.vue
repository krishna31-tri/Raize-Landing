<template>
  <div class="home">
    <div class="homeWrapper">
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
      </div>
      <div class="videoside">
        <img class="homebg" alt="Vue logo" src="../assets/backgroundhome.png" />
        <div class="video-container">
          <img class="dots" alt="Vue logo" src="../assets/dots.png" />
          <video autoplay muted>
            <source src="../assets/videoHome.mp4" type="video/mp4" />
            Your browser does not support the video tag.
          </video>
        </div>
      </div>
    </div>

    <img class="iconbg" alt="Vue logo" src="../assets/iconbg.png" />
  </div>
</template>
<script>
export default {
  name: "HomePage",
};
</script>
<style>
/* Desktop view styles (default) */
.home {
  position: relative;
}

.homeWrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  height: 650px;
  align-items: center;
  max-width: 1500px;
  margin: auto;
}

.homepage {
  display: flex;
  flex-direction: column;
}

.iconbg {
  position: absolute;
  bottom: -26%;
  left: 0%;
  z-index: -1;
  width: 131px;
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
  width: 50%;
  height: 100%;
  display: flex;
  justify-content: start;
  align-items: center;
}

.video-container {
  position: relative;
}

.video-container .dots {
  position: absolute;
  top: -5%;
  right: -4%;
  z-index: -1;
}

video {
  width: 460px;
  height: 263px;
  border-radius: 17px;
}

.homebg {
  position: absolute;
  top: 27px;
  right: 0%;
  z-index: -1;
  width: 43%;
  height: 750px;
}

/* Tablet view styles */
@media (max-width: 1024px) {
  .homeWrapper {
    flex-direction: column;
    height: auto;
    gap: 45px;
  }

  .homepage {
    text-align: center;
  }

  .iconbg {
    bottom: -15%;
    width: 100px;
  }

  .heading {
    font-size: 24px;
    padding: 20px;
    margin-left: 0;
  }

  .headingpost {
    margin-top: -30px;
    margin-left: 0;
  }

  .buttons {
    flex-direction: row;
    gap: 10px;
  }

  .genesisbutton,
  .pitchbutton {
    width: 80%;
  }
}

/* Mobile view styles */
@media (max-width: 768px) {
  .homebg {
    width: 100%;
  }

  .iconbg {
    bottom: -5%;
  }

  .videoside {
    width: 80%;
    padding: 20px;
  }

  video {
    width: 100%;
    height: auto;
  }
}
@media (max-width: 650px) {
  .buttons {
    flex-direction: column;
    align-items: center;
  }
  .pitchbutton{
    height: 70px;
    width: 164px;
  }
}
</style>
