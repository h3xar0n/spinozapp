<template>
  <div id="app">
    <!-- Top Menu -->
    <div class="top">
      <div id="nav-icon" class="menu-toggle open">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
      <img src="images/spinoza-menu.png">
      <h1>Spinoz<i>app</i></h1>
    </div>

  </div>
</template>

<script>
</script>

<style lang="scss">

  body {
    font-family: 'Agane-45', sans-serif;
    color: #1c252b;
    background-color: #f6f4ef;
    font-size: 20px;
    margin: 0;
  }

  h1, h2, h3, h4, h5, h6 {
    font-family: 'Philosopher', sans-serif;
  }

  #nav-icon {
    float: left;
    width: 30px;
    height: 30px;
    position: relative;
    margin: 10px 0 0 5px;
    -webkit-transform: rotate(0deg);
    -moz-transform: rotate(0deg);
    -o-transform: rotate(0deg);
    transform: rotate(0deg);
    -webkit-transition: .5s ease-in-out;
    -moz-transition: .5s ease-in-out;
    -o-transition: .5s ease-in-out;
    transition: .5s ease-in-out;
    cursor: pointer;
  }

  #nav-icon span {
    display: block;
    position: absolute;
    height: 3px;
    width: 100%;
    background: #d3531a;
    border-radius: 9px;
    opacity: 1;
    left: 0;
    -webkit-transform: rotate(0deg);
    -moz-transform: rotate(0deg);
    -o-transform: rotate(0deg);
    transform: rotate(0deg);
    -webkit-transition: .25s ease-in-out;
    -moz-transition: .25s ease-in-out;
    -o-transition: .25s ease-in-out;
    transition: .25s ease-in-out;
  }

  #nav-icon span:nth-child(1) {
    top: 0px;
  }

  #nav-icon span:nth-child(2),#nav-icon span:nth-child(3) {
    top: 10px;
  }

  #nav-icon span:nth-child(4) {
    top: 20px;
  }

  #nav-icon.open span:nth-child(1) {
    top: 10px;
    width: 0%;
    left: 50%;
  }

  #nav-icon.open span:nth-child(2) {
    -webkit-transform: rotate(45deg);
    -moz-transform: rotate(45deg);
    -o-transform: rotate(45deg);
    transform: rotate(45deg);
  }

  #nav-icon.open span:nth-child(3) {
    -webkit-transform: rotate(-45deg);
    -moz-transform: rotate(-45deg);
    -o-transform: rotate(-45deg);
    transform: rotate(-45deg);
  }

  #nav-icon.open span:nth-child(4) {
    top: 10px;
    width: 0%;
    left: 50%;
  }

  .top {
  background: white;
  width: 100%;
  height: 63px;
  position: fixed;
  z-index: 1001;
  padding-top: 10px;
  img {
    width: 65px;
    margin: 0 9vw;
    display: inline;
    }
  h1 {
    display: inline;
    padding-top: 40px;
    }
  }

</style>