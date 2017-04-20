<template>
  <div class='big-button-container'>
    <button
      @mousedown="buttonUp"
      @mouseup="hitIt"
    >Hit me!</button>
  </div>
</template>

<script>

  export default {
    data () {
      return {}
    },
    methods: {
      hitIt () {
        // Gpio.
        // component.writeSync(1)
        // console.log('awwwwyes')
      },
      buttonUp () {
        // component.writeSync(0)
        // console.log('buttonUp')
      }
    }
  }
</script>

<style scoped>
  .big-button-container{
    display: flex;
    justify-content: center;
    align-items: center;
  }

  button {
    background-color: orangered;
    color: white;
    font-size: 50px;
    font-weight: bold;
    display:block;
    height: 300px;
    width: 300px;
    border-radius: 50%;
    border: 1px solid orangered;
    outline: none;
    box-shadow: 4px 4px 11px -1px rgba(0,0,0,0.4);
  }

  button:hover {
    background-color: orange;
  }

  button:active {
    background-color: darkred;
    box-shadow: 0 0 0 0;
  }
</style>
