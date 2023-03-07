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
 <div>
    <p>This is an counter page</p>
    <p>{{$store.state.counter}}</p>
    <increment-counter/>
    <decrement-counter/>
    <reset-counter/>
    <set-value/>
    <router-link to='/'>Back to home</router-link>
  </div>

</template>

<script>
import incrementCounter from "@/components/incrementCounter";
import decrementCounter from "@/components/decrementCounter";
import resetCounter from "@/components/resetCounter";
import setValue from "@/components/setValue";


export default {
  components:{
    incrementCounter,
    decrementCounter,
    resetCounter,
    setValue
  }
}
</script>

