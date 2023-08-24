<template>
  <div>
    <NavBar/>
    <HomePage/>
    <CompetitiveLandscape/>
    <CompliantDesign/>
    <SubscriptionPlan/>
    <Incentive_Program/>
    
    <TeamTalented/>
    <Team_partners/>
    <FAQ/>
    <Road_Map/>
    <FooterPage/>
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
    Incentive_Program,
    TeamTalented,
    Team_partners,
    SubscriptionPlan
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
