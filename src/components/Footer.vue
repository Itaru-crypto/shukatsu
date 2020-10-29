<template>
  <div class="footer">
    <div class="footer--home">
      バーチャル就活塾
    </div>
    <nav class="nav">
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/service">Service</a></li>
        <li><a href="/about">About</a></li>
        <li><a href="/voices">Voices</a></li>
      </ul>
    </nav>
    <div>
      <h4>©️ 2020 Virtual Shukatsu All rights reserved.</h4>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Footer',
}
</script>>

<style>
.footer--home{
  text-align: center;
  margin-top: 40px;
  padding: 10px;
}
.nav a{
  text-align: center;
}
@media screen and (max-width: 768px){
  h4{
    font-size: 12px;
  }
}
</style>