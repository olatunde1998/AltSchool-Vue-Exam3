<template>
    <div>
    <button @click='increment'>Increment +</button>
    </div>
</template>
<script>
export default{
    methods:{
      increment(){
        this.$store.dispatch('increment', 10)
      }
    }
  }
</script>


