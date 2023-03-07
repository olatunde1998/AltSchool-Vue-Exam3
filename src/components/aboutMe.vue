<template lang="">
  <h3 class='about-me'>About Me 👎</h3>
  <div class='about-info'>
    <p>
      AltSchool ID: <span>{{ studentDetails.identification }}</span>
    </p>
    <p>
      Full Name: <span> {{ studentDetails.fullName }}</span>
    </p>
    <p>
      Phone Number: <span>{{ studentDetails.mobileNumber }}</span>
    </p>
    <p>
      E-mail: <span>{{ studentDetails.email }}</span>
    </p>
    <p>
      Portfolio:
      <a class='portfolio' href="https://geodev-portfolio-app.netlify.app/">{{
        studentDetails.portfolioWebsite
      }}</a>
    </p>
  </div>
</template>
<script setup>
import { reactive } from "@vue/reactivity";

const studentDetails = reactive({
  fullName: "Olatunde Rasheed",
  school: "AltSchool",
  identification: "ALT/SE/5768",
  email: "olatunde336@gmail.com",
  mobileNumber: "+2348133642798",
  portfolioWebsite: "portfolio website",
});
</script>
<style>
    .about-info{
        padding-left: 10px;
    }
    .portfolio{
        text-decoration: none;
        color: red;
    }
    .about-me{
        color: white;
    }
</style>
