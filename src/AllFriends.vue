<template>
  <div id="all-friends">
    <h2>All Friends</h2>
    <div v-for="(friend,index) in friends" :key="index">
      <span>{{friend.name}}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "AllFriends",
  data() {
    return {
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
</style>

