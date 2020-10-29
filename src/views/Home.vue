<template>
  <div id="app">
    <header>
      <Header></Header>
    </header>
    <div class="main-visual">
      <img src="../assets/5.jpg" alt="">
      <h1>答えのない世界に挑む君へ</h1>
      <button onclick="location.href='./about'">詳しく見る</button>
    </div>
    <div id="container" class="contents--wrap">
      <div id="contents">
        <div id="main">
          <section id="worries">
            <h2 class="heading2 heading2--cleaning">
              <div class="heading2--textWrap">
                <h1>こんな悩みを抱えていませんか？</h1>
              </div>
            </h2>
            <div class="worries-list">
              <div class="worries--list--left">
                <figure>
                  <img src="../assets/anxiety.jpg" alt="">    
                </figure>
              </div>
              <div class="worries--list--right">
                <div>
                  <h2>よく耳にする声</h2>
                </div>
                <ul class="comments">
                  <li >自己分析を始めたけど、何が正解何かわからない</li>
                  <li >GDを選考で初めて体験したけど、周りがレベル高すぎる</li>
                  <li >面接で自分をどう表現すればいいのかを教えて欲しい</li>
                </ul>
              </div>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div id="container" class="contents--wrap">
      <div id="contents">
        <div id="sub-main">
          <section id="videos">
            <h2 class="heading3 heading3--videos">
              <div class="heading3--textWrap">
                <h2>ぜひ一度以下の動画をご覧になってください</h2>
              </div>
            </h2>
            <div class="videos-list">
              <div class="videos_list_titles">
                <h4>ESの書き方で悩んでいる方</h4>
                <h4>GD対策で悩んでいる方</h4>
                <h4>面接対策に悩んでいる方</h4>
              </div>
              <div class="videos_list_sources">
                <iframe id="video1" width="300" height="315" src="https://www.youtube.com/embed/t2BnrcoWyXs" frameborder="50" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <iframe id="video2" width="300" height="315" src="https://www.youtube.com/embed/Qk8xGKElzu8" frameborder="50" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <iframe id="video3" width="300" height="315" src="https://www.youtube.com/embed/6EeCmiGJxDU" frameborder="50" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
              </div>
            </div>
          </section>
        </div>
      </div>
      <div>
        <div>
          <div>
            <section>
            </section>
          </div>
        </div>
      </div>
    </div>
    <footer>
      <Footer></Footer>
    </footer>
  </div>
</template>

<script>
import Header from "../components/Header";
import Footer from "../components/Footer";
export default {
  name: 'Home',
  components: {
    Header,
    Footer
  },
  methods:{
    toNextPage(){
    }
  }
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}
#nav a {
  font-weight: bold;
  color: #2c3e50;
}
#nav a.router-link-exact-active {
  color: #42b983;
}
ul{
  padding-inline-start: 20px;
}
.main-visual img{
  width: 100%;
  height: 1000px;
  position: relative;
}
.main-visual h1{
  position: absolute;
  top:  720px;
  left: 0;
  right: 0;
  margin: 0 auto;
}
.main-visual button{
  position: absolute;
  top: 760px;
  left: 0;
  right: 0;
  margin: 0 auto;
  width: 200px;
  border-radius: 10px;
  background: rgba(250, 87, 58, 0.856);
  font-size: 20px;
  font-weight: bold;
  color: white;
  padding: 15px 25px;
  margin-top: 20px;
  cursor: pointer;
  -webkit-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    -moz-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    -ms-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    -o-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
}
.main-visual button:hover{
  color: rgba(250, 87, 58, 0.856);
  background-color: white;
}
#worries{
  position: relative;
}
.worries-list{
  display: flex;
  align-items: center;
}
.worries--list--left{
  width: 130%;
}
.worries--list--left img{
  width: 80%;
  box-shadow: 0 14px 10px -8px rgba(0,0,0,.2);
}
.worries--list--right{
  width: 100%;
}
.comments{
  text-align: center;
  width: 100%;
  font-size: 22px;
}
#videos{
  background-color: lightgrey;
  justify-content: space-around;
}
.heading3--textWrap h2{
  padding: 40px;
}
.videos_list_titles{
  display: flex;
  justify-content: space-around;
}
.videos_list_sources{
  width: 100%;
  display: flex;
  justify-content: space-around;
  padding: 0 0 100px;
}
@media screen and (max-width: 480px){
  .main-visual img{
    height: 400px;
  }
  .main-visual h1{
    font-size: 16px;
    position: absolute;
    top: 350px;
  } 
  .main-visual button{
    position: absolute;
    font-size: 12px;
    width: 120px;
    top: 370px;
  }
  .heading2--textWrap h1{
    font-size: 20px;
  }
  .worries-list{
    display: block;
    align-items: center;
  }
  .worries--list--left{
    width: 100%;
    height: 150px;
  }
  .worries--list--left img{
    width: 80%;
    box-shadow: 0 14px 10px -8px rgba(0,0,0,.2);
  }
  .worries--list--right{
    width: 100%;
  }
  .worries--list--right h2{
    font-size: 16px;
  }
  .comments{
    text-align: left;
    width: 100%;
    font-size: 14px;
  }
  #videos{
    background-color: lightgrey;
    justify-content: space-around;
  }
  .heading3--textWrap h2{
    padding: 40px 0 20px 0;
    font-size: 20px;
  }
  .videos_list_titles{
    display: flex;
    justify-content: space-around;
    font-size: 8px;
  }
  .videos_list_sources{
    width: 100%;
    display: flex;
    justify-content: space-around;
    padding: 0 0 100px;
  }
  iframe{
    width: 100px;
    height: 70px;
  }
}

</style>