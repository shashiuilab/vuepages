<template>
    <div>
  <h1>{{message}}</h1>
  <button @click="changeMessage">Change Message</button>
  </div>
</template>

<script>
export default {
  props : ['message'],
  beforeCreate : function() {
        console.log("Before create");
    },
    created : function() {
        console.log("created");
    },
    beforeUpdate : function() {
        console.log("Before update");
    },
    updated : function() {
        console.log("updated");
    },
    beforeMount : function() {
        console.log("Before mount");
    },
    mounted : function() {
        console.log("Mounted");
    },
    methods : {
        changeMessage : function() {
            return this.message = "Welcome to Your New Vue.js App"
        }
    }
}
</script>

<style>
h1, h2 {
  font-weight: normal;
}
</style>
