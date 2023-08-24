<template>
  <div class="partner-ui">
    <h2 class="partner-heading">Our Partners</h2>
    <div class="partner-scroll-container">
      <div class="partner-list" ref="partnerList">
        <div
          class="partner-card"
          v-for="partner in partners"
          :key="partner.id"
        ></div>
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
}

.partner-card {
  width: 268px;
  height: 116px;
  border-radius: 6px;
  margin-right: 16px;
  background-color: #f0f0f0;
  /* Add any other styling you need */
}
</style>
