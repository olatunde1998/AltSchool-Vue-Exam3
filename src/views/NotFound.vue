<template>
  <div class="notfound-wrapper">
    <div class="notfound-box">
      <p class="text404">404</p>
      <p >page not found</p>
      <router-link to="/" class="back">Back to home</router-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.notfound-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
}
.notfound-box {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 200px;
  margin: 100px auto;
}
.back{
    text-decoration: none;
    cursor: pointer;
    margin-top: 20px;
}
.text404{
    font-size: 24px;
    margin-bottom: 0px;

}
</style>
