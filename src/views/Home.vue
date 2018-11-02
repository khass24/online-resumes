<template>
<div class="student-show">
    <header class="resume-demo-dark w-profile-image bg-img dark">
                <div class="container-fluid header-inner">
                    <div class="row vcenter">
                        <div class="col-md-4">
                            <img src="images/johndoe.jpg" alt="" class="circle inner-space-2x">
                        </div><!-- / column -->
                        <div class="col-md-8">
                            <h1 class="header-title"><span class="text-primary">HELLO!</span> I'M {{student.first}} {{student.last}}</h1>
                            <h5 class="mt-2 mb-3 opc-75">{{student.email}} - {{student.phone}}</h5>
                            <p class="lead">{{student.bio}}</p>
                            <a href="#about" class="btn btn-primary smooth-scroll mt-3"><span class="text-black">MORE ABOUT ME</span> <i class="md-icon dp14 text-black">expand_more</i></a>
                        </div><!-- / column -->
                    </div><!-- / row -->
                </div><!-- / container-fluid -->
            </header> 






  <p>{{student.email}}</p>
  <h2>{{student.phone}}</h2>
  <!-- <h2>{{student.education.start_date}}</h2>
  <h2>{{student.education.end_date}}</h2>
  <h2>{{student.eduation.university_name}}</h2>
  <h2>{{student.education.degree}}</h2>
  <h2>{{student.education.details}}</h2>
  <h2>{{student.experience.start_time}}</h2>
  <h2>{{student.experience.end_time}}</h2>
  <h2>{{student.experience.job_title}}</h2>
  <h2>{{student.experience.details}}</h2>
  <<h2>{{student.skill.skill_name}}</h2> -->





  <div class="cta bg-primary">
    <div class="container-fluid">
      <div class="row vcenter">
        <div class="col-md-8">
          <h5 class="mb-0 text-black">DOWNLOAD RESUME PDF:</h5>
            </div>
              <div class="col-md-4 text-right">
                <a href="#x" class="btn btn-outline-black m-1"><i class="md-icon dp14">file_download</i> <span>ENGLISH</span></a>
            </div>
        </div><!-- / row -->
      </div><!-- / container-fluid -->
  </div><!-- / cta -->



</div>
</template>

<style>
</style>

<script>
var axios = require('axios');

export default {
  data: function() {
    return {
      student: [],
      message: "hello"
    };
  },
  created: function() {
    axios
    .get("/api/students/1")
    .then(response => {
      this.student = response.data;
    });
  },
  methods: {},
  computed: {}
};
</script>
