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
  justify-content: center;
  height: 560px;
  align-items: center;
  max-width: 1500px;
  margin: auto;
}

.homepage {
  display: flex;
  flex-direction: column;
}

.headingpre {
  font-size: 60px;
  font-weight: 800 !important;
  font-family: 'Plus Jakarta Sans', sans-serif;
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
  margin: 0;
}

.heading span {
  margin-top: 1px;
  color: rgb(104, 104, 108);
  font-weight: 800;
}

.headingpost {
  margin-top: -45px;
  margin-left: -250px;
  background: linear-gradient(to right, #2346B8 20%, #0BAADB 100%);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
}

.buttons {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.genesisbutton {
  border: none;
  color: white;
  background: linear-gradient(to bottom, #2346B8 20%, #0BAADB 100%);
  font-size: 18px;
  border-radius: 60px;
  font-family: 'Plus Jakarta Sans', sans-serif;
  padding: 24px 36px 24px 36px;
}

.pitchbutton {
  color: #4a71f0;
  border-radius: 60px;
  background: none;
  border: 2px solid #4a71f0;
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-size: 18px;
  padding: 23px 36px 23px 36px;

}

.videoside {
  width: 50%;
  height: 81%;
  display: flex;
  justify-content: flex-start;
  align-items: flex-end;
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
  width: 100%;
  height: 315px;
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

@media (max-width: 1380px) {
  .headingpre {
    font-size: 51px;
  }
}

/* Tablet view styles */
@media (max-width: 1200px) {
  .homeWrapper {
    flex-direction: column;
    height: auto;
    gap: 45px;
  }

  .homepage {
    text-align: center;
    width: 80%;
  }

  .videoside {
    width: 80%;
    justify-content: center;
  }

  .heading {
    align-items: center;
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

  .headingpre {
    font-size: 60px;
  }

  .buttons {
    flex-direction: row;
    gap: 10px;
    width: 100%;
    margin: auto;
  }

  .genesisbutton,
  .pitchbutton {
    width: 306px;
  }
}

/* Mobile view styles */
@media (max-width: 768px) {
  .homebg {
    width: 100%;
  }

  .headingpre {
    font-size: 45px;
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

  .buttons {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
