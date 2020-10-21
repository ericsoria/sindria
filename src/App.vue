<template>
  <div id="app">
    <router-view />
  </div>
</template>
<style>
  #app {
    background-color: white;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
    height: 100vh;
  }
  body {

  }
  a, p, span, h1, h2, h3, h4, h5, label {
    color: black !important;
  }

  @media (min-width: 576px) {
    #app {
      width: 465px;
      overflow: hidden;
      border-radius: 10px;
      height: 89vh;
      margin: 5vh auto;
      -webkit-box-shadow: -2px -1px 17px 5px rgba(173,173,173,1);
      -moz-box-shadow: -2px -1px 17px 5px rgba(173,173,173,1);
      box-shadow: -2px -1px 17px 5px rgba(173,173,173,1);
      padding: 1%;
    }
  }

</style>
