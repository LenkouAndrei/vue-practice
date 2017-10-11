<template>
  <div class="component">
    <h1>The User Component</h1>
    <p>I am an awesome user</p>
    <button @click="changeName">Change my Name</button>
    <hr>
    <div class="row">
      <div class="col-xs-12 col-sm-6">
        <app-user-detail :myName="name"></app-user-detail>
      </div>
      <div class="col-xs-12 col-sm-6">
        <app-user-edit></app-user-edit>
      </div>
    </div>
  </div>
</template>

<script>
import userDetail from './userDetail.vue';
import userEdit from './userEdit.vue';

export default {
  data: function() {
    return {
      name: 'Andrey'
    };
  },

  methods: {
    changeName() {
      this.name = 'Nastya';
    }
  },

  components: {
    appUserDetail: userDetail,
    appUserEdit: userEdit
  }
}
</script>

<style lang="scss" scoped>
div {
  background-color: lightblue;
  padding: 30px;
}
</style>
