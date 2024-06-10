<template>
  <div id="app">
    <div class="mask">
      <h2>mobile only</h2>
    </div>
    <div class="header"></div>
    <div class="banner">
      <div class="txt">
        <h2>Lorem, ipsum dolor.</h2>
      </div>
      <img src="https://cdn.pixabay.com/photo/2024/03/05/10/38/boat-8614314_1280.jpg" alt="">
    </div>
    <div class="info">
      <div class="txt_wrap">
        <h2 class="title">Lorem ipsum dolor sit.</h2>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
        Omnis quos magnam eius iste nemo autem aliquam modi iure consequatur quaerat.</p><br>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
          Omnis quos magnam eius iste nemo autem aliquam modi iure consequatur quaerat.</p>
      </div>
      <img src="https://cdn.pixabay.com/photo/2022/02/25/04/11/traffic-7033509_1280.jpg" alt="">
     </div>
    <div class="footer">
      <p>2024 pwa test</p>
    </div>

  </div>
</template>

<script>

export default {
  name: 'App',
  
}
</script>

<style lang="scss">
*{
  position: relative;
  margin: 0;
  padding: 0;
}
.mask{
  position: fixed;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  background: #00000099;
  z-index: 10;
  display: flex;
  justify-content: center;
  align-items: center;
  backdrop-filter: blur(40px);
  h2{
    color: #fff;
  }

  @media (max-width: 575px) {
    display: none;
  }
}
.header{
  width: 100%;
  height: 50px;
  background: rgb(34, 125, 186);
  background-image: linear-gradient(to right top, #1f53a3, #6050af, #9546af, #c433a4, #eb128d);
}
.banner{
  position: relative;
  margin-bottom: 1.5rem;
  .txt{
    position: absolute;
    width: 90%;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    background: #00000099;
    border-radius: 10px;
    z-index: 2;
    h2{
      color: #fff;
      text-align: center;
      padding: 1rem 0;
    }
  }
  img{
    width: 100%;
    height: calc(100vh - 50px);
    object-fit: cover;
  }
}
.info{
  display: flex;
  flex-direction: column;
  align-items: center;
  img{
    width: 90%;
    object-fit: cover;
  }
  .txt_wrap{
    // border: 1px solid #fa0;
    margin: 10px 0 3rem;
  }
}
.footer{
  height: 40px;
  background: #272727;
  margin-top: 3rem;
  p{
    color: #eee;
    text-align: center;
    line-height: 40px;
  }
}
</style>
