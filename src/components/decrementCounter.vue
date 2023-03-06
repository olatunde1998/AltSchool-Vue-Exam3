<template>
    <div class="border-7 border-red-800">
    <button @click='decrement'>Decrement -</button>
    </div>
</template>
<script>
export default{
    methods:{
      decrement(){
        this.$store.dispatch('decrement', 10)
      }
    }
  }
</script>
<style>
    
</style>

