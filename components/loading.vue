<template>
  <div v-if="loading" class="loading-page"><p>Loading...</p></div>
</template>

<script>
export default {
  data: () => ({
    loading: false
  }),
  methods: {
    start() {
      this.loading = true;
      console.log('Start');
    },
    finish() {
      this.loading = false;
      console.log('Finish');
    }
  }
};
</script>

<style scoped>
.loading-page {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.1);
  text-align: center;
  padding-top: 200px;
  font-size: 30px;
  font-family: sans-serif;
  color: white;
}
</style>
