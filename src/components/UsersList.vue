<template>
  <div>
    <div class="holder">
      <ul>
        <li 
          v-for="(user, index) in users"
          :key="index"
        >
          <h2>{{index}} {{ user.name }} {{ user.age }} {{ user.job }}</h2>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'UsersList',
  data () {
    return {
      users: [
        {
          name: 'Mark Wahlberg',
          age: 47,
          job: 'Actor'
        },
        {
          name: 'Michael Jordan',
          age: 37,
          job: 'Athlet'
        },
        {
          name: 'Junior Vasquez',
          age: 54,
          job: 'DJ'
        }
      ]
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
  .holder {
    width: auto;
    box-sizing: border-box;
    h1 {
      color: green;
      font-size: 2.5em;
      font-weight: bold;
    }
    h2 {
      font-size: 16px;
    }
  }
</style>
