<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <app-user></app-user>
      </div>
    </div>
  </div>
</template>

<script>
import user from './components/user.vue';

export default {
    components: {
      appUser: user
    }
  }
</script>

<style lang="scss">
div.component {
  border: 1px solid black;
  padding: 30px;
}
</style>
