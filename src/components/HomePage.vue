<template>
  <div id="body">
    <div id="wrapper"></div>
    ¨
    <div id="product-wrapper1">
      <div id="nav">Här kan kanske nav ligga</div>
      <span id="text1">Här står det lite text om nånting</span>
      <div id="product-pic1">img</div>
      <div id="overlay1"></div>
    </div>
    <div id="product-wrapper2">
      <span id="text2">Här står det lite text om nånting</span>
      <div id="product-pic2">img</div>
      <div id="overlay2"></div>
    </div>
    <div id="footer">
      <span class="nav-buttons">test test test test</span>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    props: {
      msg: String
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #wrapper {
    background-color: #777978;
    position: absolute;
    width: 1920px;
    height: 560px;
    left: 0px;
    top: 0px;
  }

  #nav {
    position: absolute;
    width: 1920px;
    top: 560px;
    background: #202020;
    left: 0px;
    margin: 0%;
  }

  #product-pic1 {
    background-color: #777978;
    position: absolute;
    width: 540px;
    height: 716px;
    left: 982px;
    top: 780px;
    box-shadow: -8px 8px 21px rgba(0, 0, 0, 0.25);
  }

  #overlay1 {
    background-color: #353535;
    position: absolute;
    width: 329px;
    height: 324px;
    left: 818px;
    top: 1334px;
  }

  #text1 {
    position: absolute;
    width: 410px;
    height: 199px;
    left: 268px;
    top: 1046px;
  }

  #product-pic2 {
    background-color: #777978;
    position: absolute;
    width: 606px;
    height: 813px;
    left: 358px;
    top: 1771px;
    box-shadow: -8px 8px 21px rgba(0, 0, 0, 0.25);
  }

  #overlay2 {
    background-color: #353535;
    position: absolute;
    width: 329px;
    height: 324px;
    left: 800px;
    top: 2422px;
  }

  #text2 {
    position: absolute;
    width: 410px;
    height: 199px;
    left: 1152px;
    top: 2019px;
  }

  #footer {
    position: absolute;
    width: 1920px;
    height: 376px;
    left: 0px;
    top: 2907px;
    background-color: #333333;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  #nav-buttons {
    background-color: rgb(168, 62, 255);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    padding: 10px;
    justify-content: center;
  }
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
</style>

<script>
  export default {}
</script>
