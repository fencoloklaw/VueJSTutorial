<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Hello World!"/>
    <employee-table v-bind:employees="employees" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import EmployeeTable from './components/EmployeeTable.vue';

export default {
  name: 'app',
  components: {
    HelloWorld,
    EmployeeTable,
  },
  data() {
    return {
      employees: [
        {
          id: 1,
          name: 'Richard Hendricks',
          email: 'richard@piedpiper.com',
        },
        {
          id: 2,
          name: 'Bertram Gilfoyle',
          email: 'gilfoyle@piedpiper.com',
        },
        {
          id: 3,
          name: 'Dinesh Chugtai',
          email: 'dinesh@piedpiper.com',
        },
      ],
    }
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
