<template lang="">
  <h3 class='technology-used'>Techonlogy used</h3>
  <div class="skill-box">
    <div class="html-box">
      <div class="html-img">
        <img src="@/assets/html.png" alt="" width="50" height="50" />
      </div>
      <p>HTML</p>
    </div>
    <div class="html-box">
      <div class="html-img">
        <img src="@/assets/css.png" alt="" width="50" height="50" />
      </div>
      <p>CSS</p>
    </div>
    <div class="html-box">
      <div class="html-img">
        <img src="@/assets/vuejs-logo.png" alt="" width="50" height="50" />
      </div>
      <p>VueJs</p>
    </div>
    <div class="html-box">
      <div class="html-img">
        <img src="@/assets/vuex.png" alt="" width="50" height="50" />
      </div>
      <p>Vuex</p>
    </div>
    <div class="html-box">
      <div class="html-img">
        <img src="@/assets/vercel.png" alt="" width="100" height="50" />
      </div>
      <p>Vercel</p>
    </div>
    <div class="html-box">
      <div class="html-img">
        <img src="@/assets/git-github.png" alt="" width="100" height="50" />
      </div>
      <p>Git & Github</p>
    </div>
  </div>
</template>
<script></script>
<style>
.skill-box {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}
.html-box {
  border: .5px solid #4a9edb;
  width: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
}
.html-img{
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #A5CFED;


}
.technology-used{
  color: #4A9EDB;
  padding-left: 10px;


}
</style>
