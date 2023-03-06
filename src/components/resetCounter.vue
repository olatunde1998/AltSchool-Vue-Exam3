<template>
    <div>
    <button @click='reset'>Reset</button>
    </div>
</template>
<script>
export default{
    methods:{
      reset(){
        this.$store.dispatch('reset', 0)
      }
    }
  }
</script>


