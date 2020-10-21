<template>
  <div style="height: 100vh; display: flex; align-items: center; justify-content: center; flex-direction: column">
      <img src="../assets/img/watermelon.png" width="40" style="margin-bottom: 10px">
      <h3 style="margin-bottom:  10%; font-weight: 800">A simplest shopping list.</h3>
      <div class="google" @click="login">Continue with Google</div>
  </div>
</template>
<script>
  import firebase from  'firebase';
  export default {
    methods: {
      login() {
        const provider = new firebase.auth.GoogleAuthProvider();
        firebase.auth().signInWithPopup(provider).then( result => {
          this.$store.dispatch("fetchUser", result.user);
          this.$router.replace({ name: "app" });
        }).catch(function(error) {
          console.log(error)
        });
      }
    }
  }
</script>
<style>
.google {
  user-select: none;
  transition: background 20ms ease-in 0s;
  cursor: pointer;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  white-space: nowrap;
  height: 36px;
  border-radius: 3px;
  color: white;
  font-size: 14px;
  line-height: 1;
  padding-left: 12px;
  padding-right: 12px;
  font-weight: 500;
  background: rgb(225, 98, 89);
  border: 1px solid rgb(190, 86, 67);
  box-shadow: rgba(15, 15, 15, 0.1) 0px 1px 2px;
  margin-bottom: 4px;
  width: 50%;
}
</style>
