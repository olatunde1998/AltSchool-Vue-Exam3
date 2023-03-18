<template lang="">
  <h3 class="about-me">About Me 👎</h3>
  <ul class="about-info">
    <li>
      AltSchool ID: <span>{{ studentDetails.identification }}</span>
    </li>
    <li>
      Full Name: <span> {{ studentDetails.fullName }}</span>
    </li>
    <li>
      Phone Number: <span>{{ studentDetails.mobileNumber }}</span>
    </li>
    <li>
      E-mail: <span>{{ studentDetails.email }}</span>
    </li>
    <li>
      Portfolio:
      <a class="portfolio" href="https://geodev-portfolio-app.netlify.app/">{{
        studentDetails.portfolioWebsite
      }}</a>
    </li>
  </ul>
</template>
<script setup>
import { reactive } from "@vue/reactivity";

const studentDetails = reactive({
  fullName: "Rasheed Olatunde",
  school: "AltSchool",
  identification: "ALT/SOE/022/5768",
  email: "olatunde336@gmail.com",
  mobileNumber: "+2348133642798",
  portfolioWebsite: "portfolio website",
});
</script>
<style>
.about-info {
  padding-left: 10px;
  color: rgb(81, 71, 71);
  font-weight: 200;
}
.portfolio {
  text-decoration: none;
  color: rgb(81, 71, 71);
}
.about-me {
  color: white;
}
li {
  margin-top: 16px;
  margin-left: 10px;
}
</style>
