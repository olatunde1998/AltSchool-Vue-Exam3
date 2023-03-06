<template>
<header>
    <img
      alt="AltSchool logo"
      class="logo"
      src="@/assets/altschool.png"
      width="125"
      height="125"
    />
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/counter">Counter</RouterLink>
        <img
          alt="rasheed logo"
          class="rasheed-img"
          src="@/assets/rasheed_img.png"
          width="125"
          height="125"
        />
      </nav>
    </div>
  </header>
  <main>
    <h3 class='text-red-800 font-bold border-2 border-red-800'>
      Welcome to Rasheed Olatunde <br />
      AltSchool Third Semester Project
    </h3>
    <p>
      As the name suggests, AltSchool Africa is different from the traditional
      institutions. We are a school for individuals looking to gain technical
      skills and kickstart a career in Tech. AltSchool Africa takes a
      non-traditional approach to learning by teaching courses directly
      connected with the selected track.
    </p>
    <p>
      In March 2022, Gov. Ugwuanyi inaugurated 34 brand new model Customary
      Courts (two per local government) across the 17 local government areas of
      the state. Below are some facilities of the State Judiciary:
    </p>
    <!-- about the student-->
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
      <a href="https://geodev-portfolio-app.netlify.app/">{{
        studentDetails.portfolioWebsite
      }}</a>
    </p>
  </main>
</template>

<script setup>
import { reactive } from "@vue/reactivity";

const studentDetails = reactive({
  fullName: "Olatunde Rasheed",
  school: "AltSchool",
  identification: "ALT/SE/5768",
  email: "olatunde336@gmail.com",
  mobileNumber: "+2348133642798",
  portfolioWebsite: "https://geodev-portfolio-app.netlify.app/",
});

</script>


<style>
header {
  line-height: 1.5;
  max-height: 100vh;
  display:flex;
  justify-content: space-between;
}

.logo {
    margin: 0 2rem 0 0;
    width:70px;
    height:70px;
  }
.rasheed-img{
  border-radius:50%;
  border:2px solid gray;
  width:32px;
  height:32px;
  margin-right:30px;
  
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
  display:flex;
  align-items: center;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    justify-content: space-between;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}

</style>