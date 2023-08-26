<template>
  <div class="partner-ui">
    <img class="partnerbg" alt="Vue logo" src="../assets/incentivebg.png" />
    <div class="partner-ui-div">
      <h2 class="partner-heading">Our Partners</h2>
      <p>Short description goes here</p>
      <div class="partner-scroll-container">
        <div class="partner-list" ref="partnerList">
          <div class="partner-card" v-for="partner in partners" :key="partner.id"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Team_partners',
  data() {
    return {
      partners: [
        { id: 1 },
        { id: 2 },
        { id: 2 },
        { id: 2 },
        { id: 2 },

        { id: 2 },
        { id: 2 },
        { id: 2 },
        { id: 2 },
        { id: 2 },
        { id: 2 },
        // Add more partner data as needed
      ],
    };
  },
  mounted() {
    const partnerList = this.$refs.partnerList;
    partnerList.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      // Handle scrolling logic here
    },
  },
};
</script>

<style scoped>
.partner-ui {
  position: relative;
  padding: 9% 0%;
}

.partner-ui-div {
  padding: 16px;
}

.partner-heading {
  font-size: 24px;
  margin-bottom: 16px;
}

.partner-scroll-container {
  overflow-x: auto;
}

.partner-list {
  display: flex;
  flex-wrap: nowrap;
  width: fit-content;
  overflow: scroll;
}

.partner-list::-webkit-scrollbar {
  width: 0.5em;
  /* Set a small width to make the pseudo-element active */
  height: 0.5em;
  /* Set a small height to make the pseudo-element active */
}

.partner-list::-webkit-scrollbar-thumb {
  background-color: transparent;
  /* Make the scrollbar thumb transparent */
}

.partnerbg {
  position: absolute;
  top: 0;
  left: 0;
  width: 97%;
  z-index: -1;
  height: 100%;
}

.partner-card {
  width: 200px;
  height: 116px;
  border-radius: 6px;
  margin-right: 16px;
  background-color: #f0f0f0;
  /* Add any other styling you need */
}


/* Responsive Styles */
@media (max-width: 768px) {
  .partner-ui {
    padding: 6% 0;
    /* Adjust padding for smaller screens */
  }

  .partner-heading {
    font-size: 20px;
    /* Adjust font size for smaller screens */
  }

  .partner-card {}
}</style>
