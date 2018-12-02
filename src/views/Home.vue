<template>
  <div class="home page">
    <h1>This is a home page</h1>
    <UsersList></UsersList>
  </div>
</template>

<script>
import UsersList from '../components/UsersList.vue';
export default {
  components: {
    UsersList
  }
};
</script>

<style scoped lang="less">
  .home {
    background: #c3e63e;
    border-radius: 10px;
    padding-left: 10px;
    margin-top: 10px;
    padding-right: 10px;
    box-sizing: border-box;
  }
</style>
