<template>
  <div class="flex-container">
    <div class="text-wrap">
      <div class="text-item">
        <h2>Lorem, ipsum.</h2>
      </div>
      <div class="text-item">
        <h1>Lorem ipsum dolor sit.</h1>
      </div>
    </div>
    <div class="main-img">
      <img src="https://picsum.photos/900/700" width="900" height="700" alt=""></div>
  </div>
</template>

<style>
  .main-img {
    width: 80%;
    margin-top: 15px
  }

  .text-wrap {
    width: 20%;
    position: relative;
  }

  .text-wrap .text-item {
    position: absolute;
    top: 150px;
    left: 100px;
  }

  .text-wrap .text-item:nth-child(1){
    width: 100px;
  }

  .text-wrap .text-item:nth-child(2){
    top: 300px;
    width: 240px;
  }


.text-wrap .text-item h1 {
  background: #ffffff;
  padding: 6px;
  text-transform: uppercase;
  display: inline;
  font-size: 46px;
  letter-spacing: 11px;
  font-family: 'Gruppo';
}

.text-wrap .text-item h2 {
  background: #ffffff;
  font-family: 'Gruppo';
}

@media only screen and (max-width: 480px){
.text-wrap .text-item:nth-child(1) h2 {
    font-family: 'Gruppo';
    font-size: 29px;
    display: inline;
    background: #ffffff;
    letter-spacing: 8px;
  }

  .text-wrap {
    width: 0;
  }

  .text-wrap .text-item:nth-child(1) {
    left: 20px;
  }

  .text-wrap .text-item:nth-child(2) {
    left: 10px;
  }

  body {
    overflow-x: hidden;
  }
}
</style>
