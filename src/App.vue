<template>
  <div>
    <NavBar />
    <MobileNav />
    <HomePage />
    <CompetitiveLandscape />
    <MobilecompetitveLandscape />
    <CompliantDesign />
    <SubscriptionPlan />
    <MobileSubscription />
    <Incentive_Program />
    <TeamTalented />
    <Team_partners />
    <FAQ />
    <DesktopRoadmap />
    <RoadMap />
    <FooterPage />

  </div>
</template>

<script>

import HomePage from './components/HomePage.vue'
import CompetitiveLandscape from './components/competitiveLandscape.vue';
import CompliantDesign from './components/compliantDesign.vue';
import FAQ from './components/FAQ.vue';
import TeamTalented from './components/teamtalented.vue'
import Incentive_Program from './components/incentiveProgram.vue'


import Team_partners from './components/partners.vue';
import FooterPage from './components/footer.vue'
import NavBar from './components/NavBar.vue';
import SubscriptionPlan from './components/subscriptionPlan.vue';
import DesktopRoadmap from './components/DesktopRoadmap.vue';
import RoadMap from './components/RoadMap.vue';
import MobileSubscription from './components/MobileSubscription.vue';
import MobilecompetitveLandscape from './components/MobilecompetitveLandscape.vue';
import MobileNav from './components/MobileNav.vue';
export default {
  name: 'App',
  components: {
    HomePage,
    CompetitiveLandscape,
    CompliantDesign,
    FAQ,
    FooterPage,
    RoadMap,
    Incentive_Program,
    TeamTalented,
    Team_partners,
    NavBar,
    SubscriptionPlan,
    DesktopRoadmap,
    MobileSubscription,
    MobilecompetitveLandscape,
    MobileNav
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300&display=swap');

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  font-family: 'Plus Jakarta Sans';
}

button {
  font-family: 'Plus Jakarta Sans', sans-serif;
}
</style>
