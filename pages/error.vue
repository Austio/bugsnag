<template>
  <div>
    <button @click="throwError">
      Throw an error
    </button>
  </div>
</template>

<script>
  export default {
    name: 'IndexPage',
    methods: {
      throwError() {
        throw(new Error('this is a new error'));
      }
    },
    created() {
      if (this.$route.query.error) {
        this.throwError();
      }
    }
  }
</script>

<style scoped>
  .title {
    text-align: center;
    font-weight: 200;
  }
  .svg {
    margin: 0 auto;
    align: center;
    max-width: 50%;
  }
</style>
