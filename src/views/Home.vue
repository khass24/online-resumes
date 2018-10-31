<template>
  <div class="home">
    <div v-for="student in students">{{ student }}</div>  
  </div>
</template>

<style>
</style>

<script>
// var axios = require('axios');

export default {
  data: function() {
    return {
      student: {
        first: [],
        last: [],
        email: [],
        phone: [],
        bio: [],
        link: [],
        twitter: [],
        website: [],
        resume: [],
        github: [],
        photo: []
      },
      experience: {
        start_date: [],
        end_date: [],
        job_title: [],
        company_name: [],
        details: []
      },
      education: {
        start_date: [],
        end_date: [],
        degree: [],
        university_name: [],
        details: []
      },
      skills: {
        skill_name: []
      }
    };
  },
  created: function() {
    axios
    .get("http://localhost:3000/api/students" + this.$route.params.id)
    .then(response => {
      this.student = response.data;
    });
  },
  methods: {},
  computed: {}
};
</script>
