<template>
  <div class="navbar">
    <div class="logo">
      <img alt="Vue logo" src="../assets/raiseLogo.png">
    </div>
    <div class="navitems">
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
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    msg: String
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

  align-items: center;

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
.launchbutton {
  border: none;
  color: white;
  background-color: rgba(74, 113, 240, 1);
  height: 40px;
  width: 140px;
  font-size: 15px;
  border-radius: 20px;
}

@media(max-width:1100px) {
  .navbar {
    display: none;
  }
}
</style>
