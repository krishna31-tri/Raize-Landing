<template>
  <div class="navbar">
    <div class="logo">
      <img alt="Vue logo" src="../assets/raiseLogo.png">
    </div>
    <div :class="['navitems', { 'mobile-menu-open': isMobileMenuOpen }]">
      <span>Competition</span>
      <span>Compliance</span>
      <span>Pricing</span>
      <span>Incentive</span>
      <span>Team</span>
      <span>Partners</span>
      <span>FAQ</span>
    </div>
    <div>
      <button class="launchbutton">Launch App</button>
    </div>
    <!-- Hamburger icon for tablets only -->
    <div class="hamburger tablet-hamburger" @click="toggleMobileMenu">
      <div class="bar"></div>
      <div class="bar"></div>
      <div class="bar"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    msg: String
  },
  data() {
    return {
      isMobileMenuOpen: false
    };
  },
  methods: {
    toggleMobileMenu() {
      this.isMobileMenuOpen = !this.isMobileMenuOpen;
    }
  }
};
</script>

<style scoped>
/* Navbar styles */
.navbar {
  display: flex;
  flex-direction: row;
  align-content: center;
  justify-content: space-around;
}

/* Logo styles */
.logo img {
  /* Your logo styles */
}

/* Navigation items styles */
.navitems {
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 35vw;
  gap: 24px;
}

.navitems span {
  /* Your navigation item styles */
}

/* Launch button styles */
.launchbutton{
  border: none;
  color: white;
  background-color: rgba(74, 113, 240, 1);
  height: 40px;
  width: 140px;
  font-size: 15px;
  border-radius: 20px;
}

/* Hamburger icon styles */
.tablet-hamburger {
  display: none;
  cursor: pointer;
}

.bar {
  width: 25px;
  height: 3px;
  background: rgba(74, 113, 240, 1);
  margin: 3px 0;
  transition: transform 0.3s;
}

.mobile-menu-open .bar:nth-child(1) {
  transform: translateY(7px) rotate(45deg);
}

.mobile-menu-open .bar:nth-child(2) {
  opacity: 0;
}

.mobile-menu-open .bar:nth-child(3) {
  transform: translateY(-7px) rotate(-45deg);
}

/* Media query for tablet view */
@media screen and (max-width: 1200px) {
  .navitems {
    display: none;
  }

  .hamburger {
    display: none;
  }
  .launchbutton {
    margin-left: 400px; /* Adjust the margin as needed */
  }

  .tablet-hamburger {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
}
</style>
