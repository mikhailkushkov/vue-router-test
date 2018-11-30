<template>
  <div id="app">
    <div id="nav">
      <router-link to="/" class="link active">Home</router-link> |
      <router-link to="/about" class="link">About</router-link> |
      <router-link to="/contact" class="link">Contact</router-link> |
      <router-link to="/testLink" class="link">Test-Link</router-link>
    </div>
    <transition name="router-anim">
      <router-view/>
    </transition>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  components: {
    HelloWorld,
  },
};
</script>

<style lang="less">
  body {
    background: rgb(233, 233, 233);
    font-family: Arial, Helvetica, sans-serif;
  }
  html, body {
    height: calc(100% - 50px);
  }
  #app {
    background: #fff;
    width: 50%;
    padding: 30px;
    border-radius: 10px;
    margin: 50px auto 0 auto;
    height: calc(60% - 50px);
  }
  .page {
    position: fixed;
    width: calc(50% - 60px);
  }
  .router-anim-enter-active {
    animation: coming 1s;
    animation-delay: .5s;
    opacity: 0;
  }
  .router-anim-leave-active {
    animation: going 1s;
  }
  @keyframes going {
      from {
        transform: translateX(0);
      }
      to {
        transform: translateX(-50px);
        opacity: 0;
      }
    }
  @keyframes coming {
    from {
      transform: translateX(-50px);
      opacity: 0;
    }
    to {
      transform: translateX(0px);
      opacity: 1;
    }
  }
  .link {
    color: #fff;
    font-weight: lighter;
    text-decoration: none;
    padding: 3px 5px;
    background: #8990f1;
    border-radius: 5px;
    &:hover {
      text-decoration: unset;
      color: #fff;
    }
  }
  .router-link-exact-active {
    background: cyan;
  }
</style>

