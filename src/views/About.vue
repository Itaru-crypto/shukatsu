<template>
  <div>
    <header>
      <Header></Header>
    </header>
    <main>
      <div id="container">
        <div class="about--title">
          <h1>バーチャル就活塾について</h1>
        </div>
        <div class="explanation">
          <div class="expl--left">
            <img src="../assets/twitter_icon.jpg" alt="アイコンの画像"/>
          </div>
          <div class="expl--right">
            <h2>プロフィール</h2>
            <p>どうもバーチャル就活塾運営者です！当サイトをご覧いただき、有難うございます。
            神戸大学出身で21卒です。内定先は大手コンサルティングファームです。
            就活は早めに終わったので、自分の経験を活かして皆さんのお役に立ちたいと思い、このサービスを始めました。このサービスの特徴としては小手先の技術ではなく、面接官に響くESの書き方やGDでの考え方などを発信しています。就活に少なからず不安を抱いている人が大半だと思います。少しでもこのサービスに興味を持っていただければ、幸いです。それでは一緒に頑張りましょう！！</p>
          </div>
        </div>
      </div>
      <div class="common-questions">
        <div class="questions-title">
          <h1>よくある質問</h1>
        </div>
        <div class="questions-contents">
          <div class="question1"> 
            <h3>Q1. 入会するのにお金はかかりますか？</h3>
            <h5>A. はい。入会の時点でお金を支払いいただいて、その後にサービスを利用していただけるようになります。費用に関してましては一括だけでなく、分割支払いでも承っています。</h5>
          </div>
          <div class="question2"> 
            <h3>Q2. 入会までの流れは?</h3>
            <h5>GD練習会の見学</h5>
            <a class="arrow_u"></a>
            <h5>ES添削の体験</h5>
            <a class="arrow_u"></a>
            <h5>電話面談による入会の意思確認</h5>
            <a class="arrow_u"></a>
            <h5>入会決定</h5>
            <h5>この流れが基本的には入会までの手順となっています。ご本人の意思によっては、変更が可能ですのでご相談ください。</h5>
          </div>
          <div class="question3"> 
            <h3>Q3. 会員になれば何ができますか？</h3>
            <h5>A. プランにもよりますが、GD練習会の参加、ES添削、動画コンテンツの利用、面接対策が主な内容になります。他にもチャットによる就活相談も受け付けています。</h5>
          </div>
          <div class="question4"> 
            <h3>Q4. 期間はいつまでですか？</h3>
            <h5>A. 内定獲得までがサポートの対象になります。そのため、早い時期に初めていただくと有効に活用できるというのがこのサービスの売りです。</h5>
          </div>
          <div class="question5"> 
            <h3>Q5. コミュニティですか？</h3>
            <h5>A. いえ。基本的に1対1のコンサル形式での支援になります。</h5>
          </div>
        </div>
      </div>
    </main>
    <footer>  
      <Footer></Footer>
    </footer>
  </div>
</template>
<script>
import Header from '../components/Header';
import Footer from '../components/Footer';
export default {
  name: 'About',
  components: {
    Header,
    Footer
  }
}
</script>
<style>
.explanation{
  display: flex;
}
.expl--left{
  width: 50%;
}
.expl--right{
  width: 40%;
}
.expl--left img{
  border-radius: 50%;
}
.expl--right{
  border: 5px dotted;
  border-radius: 50%;
  background-color: rgb(252, 224, 201);
}
.expl--right h2{
  margin-top: 40px;
  margin-bottom: 60px;
}
.expl--right p{
  line-height: 1.2;
  width: 90%;
  margin: 5rem auto;
}
.common-questions{
  margin-top: 150px;
  padding-bottom: 50px;
  background-color: lightcyan;
}
.questions-title{
  text-align: center;
}
.questions-contents{
  width: 60%;
  margin: 0 auto;
  text-align: center;
}
.question2 h5{
  text-align: center;
}
.question1,
.question2,
.question3,
.question4{
  margin-bottom: 50px;
}
.arrow_u {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  color: #333;
  text-decoration: none;
}
.arrow_u:before {
  content: '';
  width: 6px;
  height: 6px;
  border: 0;
  border-bottom: solid 2px #333;
  border-right: solid 2px #333;
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  margin: 0 auto;
  transform: rotate(45deg);
}
h3{
  color: #333;
}
h5{
  font-size: 20px;
}
@media screen and (max-width: 768px){
  .about--title{
    font-size: 14px;
  }
  .explanation{
    display: block;
  }
  .expl--left{
    width: 100%;
  }
  .expl--left img{
    width: 80%;
  }
  .expl--right{
    margin-top: 3rem;
    width: 100%;
  }
  .expl--right h2{
    margin-bottom: 1rem;
  }
  .expl--right p{
    font-size: 12px;
    padding-bottom: 1rem;
  }
  h3{
    color: red;
  }
  h5{
    font-size: 14px;
  }
}
</style>
