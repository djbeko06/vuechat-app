<template>
  <div id="app">
    <h1>{{title}}</h1>
    <h2>Menu</h2>
    <Navbar/>
    <AllFriends/>
    <OnlineFriends/>
  </div>
</template>

<script>
import Navbar from "./Navbar";
import AllFriends from "./AllFriends";
import OnlineFriends from "./OnlineFriends";

export default {
  name: "app",
  components: {
    Navbar,
    OnlineFriends,
    AllFriends
  },
  data() {
    return {
      title: "My first Vue app, wohoo :)"
    };
  }
};
</script> 

<style>
h1,
h2 {
  color: #444;
  font-weight: normal;
  text-align: center;
}
</style>
