<template>
  <div id="Header">
    <div class="header">
      <h3 class="header-logo" onclick="location.href='/'">
        バーチャル就活塾
      </h3>
      <nav class="header-nav">
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/service">Service</a></li>
          <li><a href="/about">About</a></li>
          <li><a href="/voices">Voices</a></li>
        </ul>
      </nav>
    </div>
    <div id="hamburger" @click="naviOpen" :class="{'is-Active': active}">
        <span></span>
        <span></span>
        <span></span>
    </div>
    <transition name="navi">
      <nav class="navi" v-show="navi">
        <ul class="navi_wrap">
          <li><a href="/">Home</a></li>
          <li><a href="/service">Service</a></li>
          <li><a href="/about">About</a></li>
          <li><a href="/voices">Voices</a></li>
        </ul>
      </nav>
    </transition>
  </div>  
</template>
<script>
export default {
  name: 'Header',
  data(){
    return {
      active: false,
      navi: false,
    }
  },
  methods: {
    naviOpen(){
      this.active = !this.active;
      this.navi = !this.navi;
    }
  }
}
</script>
<style>
.header{
  display: flex;
  justify-content: space-between;
  height: 70px;
  background: rgb(109, 131, 131);
}
.header-logo{
  margin-left: 30px;
  color: #ffffff;
}
.header-logo:hover{
  cursor: pointer;
}
.header-nav{
  display: inline-block;
  list-style: none;
}
li{
  list-style: none; 
  display: inline-flex;
  margin-right: 30px;
  margin-top: 5px;
}
.header-nav a{
  color: #ffffff;
}
@media screen and (max-width: 768px){
  .header-logo{
    margin-left: 10px;
    margin-top: 25px;
    width: 40%;
    font-size: 12px;
  }
  .header-nav{
    display: none;
  }
  #hamburger {
    width: 40px;
    height: 70px;
    position: absolute;
    cursor: pointer;
    z-index: 100;
    top: 25px;
    right: 20px;
    transition: 0.4s;
  }
  #hamburger span {
    position: absolute;
    left: 2px;
    display: block;
    width: 35px;
    height: 2px;
    background-color: #fff;
    transition: 0.8s;
  }
  #hamburger span:nth-of-type(1) {
    top: 10px; 
  }
  #hamburger span:nth-of-type(2) {
    top: 20px; 
  }
  #hamburger span:nth-of-type(3) {
    top: 30px;
  }
  .navi-wrap li{ 
    display: block;
  }
  .header {
  width: 100%;
  height: 60px;
  }
}
</style>