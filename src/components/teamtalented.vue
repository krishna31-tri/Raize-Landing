<template>
    <div class="team-section">
      <h2 class="team-heading">Our Talented Team</h2>
      <div class="team-cards">
        <div v-for="(member, index) in teamMembers" :key="index" class="team-card">
          <div class="member-image">
            <img :src="member.image" alt="Member's Photo" />
          </div>
          <div class="member-details">
            <h3>{{ member.name }}</h3>
            <p class="job-title">{{ member.jobTitle }}</p>
            <p class="job-description">{{ member.jobDescriptionLine1 }}</p>
            <p class="job-description">{{ member.jobDescriptionLine2 }}</p>
            <div class="social-icons">
              <a v-for="(social, iconIndex) in member.socialMedia" :key="iconIndex" :href="social.link" class="social-icon">
                <img :src="social.icon" :alt="social.name" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import teamImage from '../assets/teamImage.png'
  import teamImage2 from '../assets/teamImage2.png'
  import teamImage3 from '../assets/teamimage3.png'
  import teamImage4 from '../assets/teamImage4.png'
  import LinkedInIcon from '../assets/linkedinIconTeam.png'
  import TwitterIcon from '../assets/TwitterIconTeam.png'
  import YoutubeIcon from '../assets/Youtubeicon.png'
  export default {
    name:'TeamTalented',
    data() {
      return {
        teamMembers: [
          {
            image: teamImage,
            name: 'Jean-Raphaël Sauvonnet',
            jobTitle: 'Web Developer',
            jobDescriptionLine1: 'Experienced web developer...',
            jobDescriptionLine2: 'Specialized in front-end...',
            socialMedia: [
              { name: 'LinkedIn', icon: LinkedInIcon, link: 'linkedin.com/' },
              { name: 'Twitter', icon: TwitterIcon, link: 'twitter.com' },
              { name: 'You Tube', icon: YoutubeIcon, link: 'youtube.com' }
            ],
          },
          {
            image: teamImage2,
            name: 'Jean-Raphaël Sauvonnet',
            jobTitle: 'Web Developer',
            jobDescriptionLine1: 'Experienced web developer...',
            jobDescriptionLine2: 'Specialized in front-end...',
            socialMedia: [
              { name: 'LinkedIn', icon: LinkedInIcon, link: 'linkedin.com/' },
              { name: 'Twitter', icon: TwitterIcon, link: 'twitter.com' },
              { name: 'You Tube', icon: YoutubeIcon, link: 'youtube.com' }
            ],
          },
          {
            image: teamImage3,
            name: 'Jean-Raphaël Sauvonnet',
            jobTitle: 'Web Developer',
            jobDescriptionLine1: 'Experienced web developer...',
            jobDescriptionLine2: 'Specialized in front-end...',
            socialMedia: [
              { name: 'LinkedIn', icon: LinkedInIcon, link: 'linkedin.com/' },
              { name: 'Twitter', icon: TwitterIcon, link: 'twitter.com' },
              { name: 'You Tube', icon: YoutubeIcon, link: 'youtube.com' }
            ],
          },
          {
            image: teamImage4,
            name: 'Jean-Raphaël Sauvonnet',
            jobTitle: 'Web Developer',
            jobDescriptionLine1: 'Experienced web developer...',
            jobDescriptionLine2: 'Specialized in front-end...',
            socialMedia: [
              { name: 'LinkedIn', icon: LinkedInIcon, link: 'linkedin.com/' },
              { name: 'Twitter', icon: TwitterIcon, link: 'twitter.com' },
              { name: 'You Tube', icon: YoutubeIcon, link: 'youtube.com' }
            ],
          },
          // Add more team members similarly
        ],
      };
    },
  };
  </script>
<style scoped>
.team-section {
  text-align: center;
  padding: 30px;
}

.team-heading {
  font-size: 36px;
  margin-bottom: 20px;
}

.team-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.team-card {
  width: 273px;
  /* height: 412px; */
  top: 141px;
  box-shadow:
    10px 10px 15px 0px rgba(74, 113, 240, 0.1),
    -10px 0px 10px 0px rgba(0, 29, 61, 0.02);
  background-color: #ffffff;
  border-radius: 10px;
  padding: 20px;
  margin: 15px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.member-image img {
    width: 160px;
    height: 160px;
    border-radius: 50%;
    margin: 0 auto 10px;
    display: block;
}

.member-details h3 {
  font-size: 18px;
  margin: 5px 0;
}

.job-title {
  font-style: italic;
  margin-bottom: 10px;
}

.job-description {
  margin-bottom: 5px;
}

.social-icons {
  display: flex;
  justify-content: center;
  margin-top: 10px;
}

.social-icon {
  display: inline-block;
  margin: 0 5px;
}

.social-icon img {
  width: 30px;
  height: 30px;
}

</style>
  