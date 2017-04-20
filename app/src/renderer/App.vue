<template>
  <div id="app">
    <div>
      <h1>Hit!</h1>
      <h1>That!</h1>
      <h1>Button!!!</h1>
    </div>
    <big-button></big-button>
  </div>
</template>

<script>
  import BigButton from './components/BigButton'

  export default {
    components: {
      BigButton
    }
  }
</script>

<style>
  @import url(https://fonts.googleapis.com/css?family=Lato:300);

  * {
    margin: 0;
    padding: 0;
  }

  html,
  body { height: 100%; }

  body {
    background:
      radial-gradient(
        ellipse at center,
        rgba(255, 255, 255, 1) 0%,
        rgba(229, 229, 229, .85) 100%
      );
    background-position: center;
    display: flex;
    font-family: Lato, Helvetica, sans-serif;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
</style>

<style scoped>
  #app {
    display: flex;
    justify-content: space-around;
    /*background-color: green;*/
    flex-direction: column;
    /*flex: 1;*/
    /*align-items: stretch;*/
  }

  #app > * {
    padding: 20px;
    /*flex: 1;*/
    /*border: 1px solid red;*/
  }
</style>
