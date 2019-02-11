<template>
  <div id="app">
    <h1>{{title}}</h1>
    <h2>Menu</h2>
    <Navbar/>
    <Blogs/>
    <!-- <AllFriends :friends="friends"/>
    <OnlineFriends :friends="friends"/> -->
  </div>
</template>

<script>
import Navbar from "./Navbar";
import Blogs from "./Blogs";
import AllFriends from "./AllFriends";
import OnlineFriends from "./OnlineFriends";

export default {
  name: "app",
  components: {
    Navbar,
    OnlineFriends,
    AllFriends,
    Blogs
  },
  data() {
    return {
      title: "My first Vue app, wohoo :)",
      friends: [
        { name: "Tinashe", online: true },
        { name: "Blessing", online: false },
        { name: "Natalie", online: true },
        { name: "Amanda", online: false }
      ]
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
