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
        <a href="https://github.com/olatunde1998/AltSchool-Vue-Exam3">Github</a>

        <div class="rasheed-box">
          <img
            alt="rasheed logo"
            class="rasheed-img"
            src="@/assets/rasheed_img.png"
            width="125"
            height="125"
          />
        </div>
      </nav>
    </div>
  </header>
  <main>
    <!-- altschool wrapper section-->
    <div class="altschool-wrapper">
      <h3 class="welcome">
        Welcome 👋 <br />
        I'm Rasheed Olatunde
      </h3>
      <div>
        <h3 class="altschool-name">AltSchool Africa Third Semester Exam </h3>
        <p class="altschool-history">
          As the name suggests, AltSchool Africa is different from the
          traditional institutions. We are a school for individuals looking to
          gain technical skills and kickstart a career in Tech. AltSchool Africa
          takes a non-traditional approach to learning by teaching courses
          directly connected with the selected track.
        </p>
      </div>
    </div>
    <div class="about-project">
      <!-- about the student-->
      <div class="about-wrapper">
        <about-me />
      </div>
      <!--project section-->
      <div class="project-wrapper">
        <project-info />
      </div>
    </div>
    <!-- skill/ technology used-->
    <div class="skills">
      <skills-used />
    </div>
  </main>
  <footer-section />
</template>

<script>
import aboutMe from "@/components/aboutMe";
import skillsUsed from "@/components/skillsUsed";
import footerSection from "@/components/footerSection";
import projectInfo from "@/components/projectInfo";

export default {
  components: {
    aboutMe,
    skillsUsed,
    footerSection,
    projectInfo,
  },
};
</script>

<style>
header {
  line-height: 1.5;
  max-height: 100vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1440px;
  vertical-align: center;
  background: #4a9edb;
}
.altschool-wrapper {
  margin-top: 30px;
}
.welcome{
  padding-left: 10px;
  margin-bottom: 50px;
}
.altschool-name{
  text-align: center;
  color: #4a9edb;
  padding-left: 0px 10px;

}
.altschool-history {
  padding:0px 10px;
  line-height:32px;
}
.logo {
  margin: 0 2rem 0 0;
  width: 60px;
  height: 60px;
}
.rasheed-img {
  border-radius: 50%;
  border: 1px solid white;
  width: 32px;
  height: 32px;

}
nav {
  font-size: 12px;
  margin-top: 2rem;
  display: flex;
  align-items: center;
  margin: auto 0;
  margin-right: 10px;
  width: 80%;
}

nav a.router-link-exact-active {
  color: #47c2e1;
  text-decoration: none;
  color: red;
}

nav a.router-link-exact-active:hover {
  color: red;
  text-decoration: none;
}

nav a {
  display: inline-block;
  padding: 0 .5rem;
  border-left: 1px solid var(--color-border);
  text-decoration: none;
  color: white;
}

nav a:first-of-type {
  border: 0;
}
main {
  max-width: 700px;
  margin: 0 auto;
}
.about-wrapper,.project-wrapper {
  background: #4a9edb;
  height: 250px;
  padding-top:10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  border-radius: 10px;
  margin: 10px 10px;
  padding:10px;
}
.about-project{
  width:100%;
  margin: 70px 0px;
}
.skills {
  margin-bottom: 70px;
  width: 100%;
}
@media (min-width: 768px) {

.about-project{
  display: flex;
  justify-content: space-between;
  width:100%;
}
.about-wrapper,.project-wrapper {
 width: 50%;
}

}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    justify-content: space-between;
    padding-right: calc(var(--section-gap) / 2);
    max-width: 1440px;
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
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
