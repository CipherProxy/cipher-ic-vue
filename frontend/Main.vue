<template>
  <div class='app'>
    <div class='header'>
       <Auth />
      <h1>Welcome!</h1>
    </div>
    <div class='content'>
      <p>{{filler}}</p>
      <button @click='displayGreeting'>Say Hello!</button>
    </div>
  </div>
</template>

<script lang="ts">
import Auth from './Auth.vue';

export default {
  name: "Main",
  // Define and instantiate your state data by stating 'yourVar: itsType'
  // Use it in HTML by {{yourData}} and in JS by using 'this.yourData'
  data: () => ({
    filler: "Content Goes Here!",
  }),
  // Define what Vue components will be loaded if any
  components: {
    Auth,
  },
  // Define your functions here to be called throughout the rest of the program
  // Use async and separate each function with a comma.
  // Call these by using 'this.yourFunctionName()' in JS or @click='' in HTML
  methods: {
    async displayGreeting() {
      alert("The page says hi back!");
    },
  }
}
</script>

<style scoped>

.app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.header {
  position: absolute;
  top: 0;
  left: 0;
  height: 70px;
  width: 100%;
  background-color: #202020;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  color: #ffcf40;
  font-size: 18px;
}

.content {
  margin-top: 100px;
  height: 500px;
  width: 700px;
  border: 1px solid gray;
  border-radius: 16px;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  font-size: 20px;
  color: #e7e7e7;
}

button {
  background: none;
  border: 1px solid #ffcf40;
  border-radius: 12px;
  font-size: 16px;
  padding: 8px 10px;
  color: lightgoldenrodyellow;
  cursor: pointer;
}

button:hover {
  background-color: rgba(255,255,255,0.1);
}

</style>
