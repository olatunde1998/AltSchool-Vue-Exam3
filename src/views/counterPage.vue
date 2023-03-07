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
  <div class="counter-wrapper">
    <div class="counter-box">
      <p class="count-heading">Counting App</p>
      <p class="count">{{ $store.state.counter }}</p>
      <div class="button-box">
        <increment-counter />
        <decrement-counter />
        <reset-counter />
      </div>
      <div class="input-value">
      <input type="number" placeholder="type your counting" />
      <set-value />
      </div>
      <router-link to="/">Back to home</router-link>
    </div>
  </div>
</template>

<script>
import incrementCounter from "@/components/incrementCounter";
import decrementCounter from "@/components/decrementCounter";
import resetCounter from "@/components/resetCounter";
import setValue from "@/components/setValue";

export default {
  components: {
    incrementCounter,
    decrementCounter,
    resetCounter,
    setValue,
  },
};
</script>
<style>
.counter-wrapper{
  border:2px solid red;
  height: 100vh;
  margin-top: 0px;
  background-color: rgb(124, 205, 214);
}
.counter-box {
  max-width: 370px;
  text-align: center;
  margin: 0 auto;
  margin-top: 60px;
  border: 2px solid green;
}
.button-box {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.count-heading{
  color:#4a9edb;

}
.count{
  font-size: 24px;
  color:#4a9edb;
}
.input-value{
  display: flex;
  justify-content: space-between;
  margin-top: 30px;
   justify-content: center;
}

</style>
