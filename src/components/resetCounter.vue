<template>
  <div>
    <button class="reset" @click="reset">Reset</button>
  </div>
</template>
<script>
export default {
  methods: {
    reset() {
      this.$store.dispatch("reset", 0);
    },
  },
};
</script>

<style>
.reset {
  padding: 12px;
  border-radius: 5px;
  background: #4a9edb;
  border: 1px solid;
  color: white;
  width: 70px;
  font-size: 16px;
}
.reset:hover {
  background: white;
  color: #4a9edb;
  border: 1px solid #4a9edb;
  border-radius: 10px;
}
</style>
