<template>
  <div>
    <NavBar />
    <HomePage />
    <CompetitiveLandscape />
    <CompliantDesign />
    <SubscriptionPlan />
    <Incentive_Program />

    <TeamTalented />
    <Team_partners />
    <FAQ />
    <Road_Map />
    <Road_Map_Desktop />
    <FooterPage />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HomePage from './components/HomePage.vue'
import CompetitiveLandscape from './components/competitiveLandscape.vue';
import CompliantDesign from './components/compliantDesign.vue';
import FAQ from './components/FAQ.vue';
import TeamTalented from './components/teamtalented.vue'
import Incentive_Program from './components/incentiveProgram.vue'
import Road_Map from './components/roadMap.vue'
import Road_Map_Desktop from './components/DesktopRoadmap.vue'
import Team_partners from './components/partners.vue';
import FooterPage from './components/footer.vue'
import SubscriptionPlan from './components/subscriptionPlan.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HomePage,
    CompetitiveLandscape,
    CompliantDesign,
    FAQ,
    FooterPage,
    Road_Map,
    Road_Map_Desktop,
    Incentive_Program,
    TeamTalented,
    Team_partners,
    SubscriptionPlan
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
  font-family: 'Plus Jakarta Sans', sans-serif;
}

button {
  font-family: 'Plus Jakarta Sans', sans-serif;
}
</style>
