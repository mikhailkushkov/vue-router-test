<template>
  <div class="about page">
    <HelloWorld></HelloWorld>

    <hr>



    <h1>This is an about page</h1>
    <p>
      Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy
      eirmod tempor invidunt ut labore et
      dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et
      justo duo dolores et ea rebum. Stet
      clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit
      amet. Lorem ipsum dolor sit amet, consetetur
      sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
      aliquyam erat, sed diam voluptua.
      At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren,
      no sea takimata sanctus est Lorem
      ipsum dolor sit amet.
    </p>
  </div>
</template>

<script>
import HelloWorld from '../components/HelloWorld.vue';

export default {
  name: 'testLink',
  components: {
    HelloWorld,
  },
};
</script>

<style scoped lang="less">
  .about {
    background: #81ecad;
    border-radius: 10px;
    padding-left: 10px;
    margin-top: 10px;
    padding-right: 10px;
    box-sizing: border-box;
  }
</style>
