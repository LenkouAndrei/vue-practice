<template>
  <div class="detail">
    <div class="row">
      <div class="col-xs-12">
        <h1>You may view the User Detail here</h1>
        <p>Many Details</p>
        <p>User Name: {{ switchName() }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    myName: {
      type: String,
      required: true
    }
  },
  methods: {
    switchName() {
      return this.myName.split('').join('-');
    }
  }
}
</script>

<style lang="scss" scoped>
  .detail {
    background-color: red;
    padding: 30px;
    border: 1px solid black;
    margin: 0;
  }
</style>
