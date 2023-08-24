<template>
  <div class="roadmap">
    <h1>Road Map</h1>
    <div class="line"></div>
    <div class="cards-container">
      <div class="center-line"></div>
      <!-- Cards above the line -->
      <div class="cards-row above">
        <div class="card" v-for="(card, index) in aboveCards" :key="index">
          <div class="vertical-line"></div>
          {{ card.title }}
        </div>
      </div>
      <!-- Cards below the line -->
      <div class="cards-row below">
        <div class="card" v-for="(card, index) in belowCards" :key="index">
          {{ card.title }}
          <div class="vertical-line"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      aboveCards: [
        { title: "Above Card 1" },
        { title: "Above Card 2" },
        { title: "Above Card 3" },
      ],
      belowCards: [
        { title: "Below Card 1" },
        { title: "Below Card 2" },
      ],
    };
  },
};
</script>

<style scoped>
.roadmap {
  text-align: center;
}

.line {
  border-top: 1px solid black;
  margin: 20px auto;
  width: 100%;
}

.cards-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
}

.cards-row {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 10px 0;
}

.center-line {
  position: absolute;
  height: 100%;
  width: 1px;
  background-color: black;
  left: 50%;
  top: 0;
  transform: translateX(-50%);
  z-index: -1;
}

.card {
  display: flex;
  align-items: center;
  position: relative;
  border: 1px solid #ccc;
  padding: 10px;
  margin: 5px;
  background-color: #f7f7f7;
}

.vertical-line {
  position: absolute;
  height: 100%;
  width: 1px;
  background-color: black;
  left: 50%;
  top: 0;
  transform: translateX(-50%);
}
</style>
