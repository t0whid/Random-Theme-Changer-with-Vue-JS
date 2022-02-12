<template>
  <div>
    <div class="container" id="root">
      <h1>Change The Theme</h1>
      <button id="change-btn" @click="generator">Change Color</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      red: 0,
      green: 0,
      blue: 0
    };
  },

  methods: {
    generator() {
      this.red = Math.floor(Math.random()*255);
      this.green = Math.floor(Math.random()*255);
      this.blue = Math.floor(Math.random()*255);
      //use this one or below one
      //document.body.style.background = "rgb("+this.red+","+this.green+","+this.blue+")"; 
      document.body.style.background = `rgb(${this.red}, ${this.green}, ${this.blue})`;

    },
  },
};
</script>

<style></style>
