<template>
  <Layout>
    
    <div class="row">
        <div class="col-md-4 d-flex flex-column justify-content-start">
          <h1 class="display-4 serif-font-face">About Super Duper Team</h1>
          <p class="font-big-1">Currently we located in Saint Petersburg</p>
            <p class="font-big-1"><g-link to="/games" class="text-dark font-weight-bold"><u>View Games</u></g-link></p>
        </div>
        <div class="col-md-8">
          <div class="row">
            <div class="col-md-4" v-for="teamMember in teamMembers"><TeamMember :team-member="teamMember" /></div>
          </div>
        </div>
    </div>

  </Layout>
</template>

<script>
import TeamMember from "../components/team/Team-Member";
export default {
    components: {TeamMember},
    metaInfo: {
    title: 'About'
    },
    data() {
        return {
            teamMembers: [
                {
                    index: 0,
                    name: "Imran Ibragimov",
                    title: "CEO & Game Developer",
                    imageSrc: "/imran.jpg",
                    description: "Waaaaaaaaaaaaaaaaaaaaaaat"
                },
                {
                    index: 1,
                    name: "Maxim Shcherbak",
                    title: "Frontend Developer & iOS",
                    imageSrc: "/insta.png",
                    description: "Hi guys"
                }
            ]
        }
    }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
