<template>
  <div id="Voices"> 
    <header>
      <Header></Header>
    </header>
    <main>
      <div id="container">
        <div class="head--title">
          <h2>利用していただいている方の声</h2>
        </div>
        <div class="real--voices">
          <div class="faceicon--left"> 
            <img id="left1" src="../assets/fivicon.png" alt="人型のアイコン"/>   
            <img id="left2" src="../assets/fivicon.png" alt="人型のアイコン"/>
          </div>
          <div class="faceicon--right">
            <img id="right1" src="../assets/fivicon.png" alt="人型のアイコン"/>            
            <img id="right2" src="../assets/fivicon.png" alt="人型のアイコン"/>
          </div>
          <div class="chatting">
            <div class="says1">
              <p>夏のインターンは全滅だったESが、添削してもらったものを提出したら通過率90%を超えました！</p> 
            </div>             
            <div class="says--right1">
              <p>GDの後にこれだけ濃いフィードバックを受けられる機会はなかなかないと思います。</p>
            </div>
            <div class="says2">
              <p>自分のガクチカや自己PRを最大限に活かした添削をしていただけるので、面接の対策にも活かしやすいです！</p> 
            </div>
            <div class="says--right2">
              <p>締め切りが迫る中、速攻で添削をしてもらえたので助かりました。自分の好きな時に見れる動画コンテンツも部活をしている身としてありがたいです。</p>
            </div>
          </div>
        </div>  
      </div>
      <div class="achievement">
        <div class="achievement--title">
          <h2>会員さんでインターンや本選考を突破した企業</h2>
        </div>
        <div class="achievement--contents">
          <ul>
            <li>NTTデータ</li>
            <li>PwCコンサルティング</li>
            <li>NTTドコモ</li>
            <li>富士通</li>
            <li>EnJapan</li>
            <li>Works Human Intelligence</li>
          </ul>
        </div>
      </div>
    </main>
    <footer>
      <Footer></Footer>
    </footer>
  </div>
</template>
<script>
import Header from "../components/Header";
import Footer from "../components/Footer";
export default {
  name: 'Voices',
  components: {
    Header,
    Footer
  }
}
</script>
<style>
#container{
  text-align: center;
}
.head--title{
  margin-bottom: 40px;
}
.real--voices{
  margin-left: 20%;
  margin-right: 20%;
  overflow: hidden;
  padding-bottom: 50px;
}
.real--voices img{
  width: 100%;
  height: auto;
}
.real--voices .faceicon--left{
  position: relative;
  float: left;
  margin-right: -50px;
  width: 40px;
}
.real--voices .faceicon--left #left1{
  margin-bottom: 160px;
}
.real--voices .faceicon--right{
  position: relative;
  float: right;
  top: 13vh;
  width: 40px;
}
.real--voices .faceicon--right #right1{
  margin-bottom: 180px;
}
.real--voices .faceicon--right #right2{
  margin-bottom: 180px;
}
.real--voices .chatting{
  width: 100%;
  text-align: left;
}
.says1,
.says2{
  display: inline-block;
  position: relative; 
  margin: 0 0 20px 50px;
  padding: 10px;
  max-width: 380px;
  border-radius: 12px;
  background: #edf1ee;
}
.says1::after,
.says2::after{
  display: inline-block;
  position: absolute;
  top: 3px; 
  left: -19px;
  border: 8px solid transparent;
  border-right: 18px solid #edf1ee;
  -webkit-transform: rotate(35deg);
  transform: rotate(35deg);
}
.says1 p,
.says2 p{
  margin: 0;
  padding: 0;
}
.says--right1,
.says--right2{
  display: inline-block;
  position: relative;
  float: right;
  padding-left: 15px;
  margin: 0 10px 20px 0;
  max-width: 380px;
  border-radius: 12px;
  background: #edf1ee;
  font-size: 15px;
}
.says--right1::after,
.says--right2::after{
  border: 8px solid transparent;
  border-left: 18px solid #edf1ee;
  -webkit-trandform: rotate(-35deg);
  transform: rotate(-35deg);
}
.achievement{
  text-align: center;
  background-image: url("../assets/selection.jpg");
  height: cover;
  background-color: lightgray;
  padding-bottom: 5rem;
}
.achievement--title{
  padding: 50px;
}
.achievement--contents li{
  padding-top: 50px;
  color: coral;
}

Footer{
  text-align: center;
}
@media screen and (max-width: 768px){
  .real--voices{
    padding-bottom: 0;
  }
  .says1{
    position: absolute;
    font-size: 10px;
    margin-right: 2rem;
  }
  .says--right1{
    position: absolute;
    font-size: 10px;
    top: 250px;
    margin-left: 2rem;
    right: 8rem;
  }
  .says2{
    position: absolute;
    top: 350px;
    font-size: 10px;
    margin-right: 2rem;
  }
  .says--right2{
    position: absolute;
    font-size: 10px;
    top: 450px;
    margin-left: 2rem;
    right: 8rem;
  }
  .achievement--title{
    padding: 0 2rem;
  }
  .achievement{
    background-image: none;
  }
}
</style>