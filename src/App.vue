<script setup>
import { ref } from "vue";
import Header from "./components/Header.vue";
import Card from "./components/Card.vue";
import CardLarge from "./components/CardLarge.vue";
import StoreInfo from "./components/StoreInfo.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";

const card = ref({
  car: {
    title: "車の内装クリーニング・洗車",
    contents:
      "お車の内装クリーニングのついでに外装ピカピカにしませんか、洗車・コーティングも承ります。",
    targetUrl: "",
    src: "/car.jpeg",
    alt: "",
  },
  extereor: {
    title: "エクステリア掃除",
    contents:
      "汚れやカビの除去、塗装のメンテナンスなどを行い、お住まいの外観を蘇らせます。",
    targetUrl: "",
    src: "https://placehold.jp/3d4070/ffffff/300x300.png",
    alt: "",
  },
  weeding: {
    title: "草取り・草刈り<br />除草剤の散布",
    contents:
      "気付くと繁殖している雑草。美しい庭を保つため、雑草対策を行います。",
    targetUrl: "",
    src: "https://placehold.jp/3d4070/ffffff/300x300.png",
    alt: "",
  },
  window: {
    title: "側溝掃除<br />網戸の張替え",
    contents: "体力を使う側溝の掃除や網戸の張替えも私たちにお任せください。",
    targetUrl: "",
    src: "https://placehold.jp/3d4070/ffffff/300x300.png",
    alt: "",
  },
  shoveling: {
    title: "雪かき",
    contents:
      "雪かきには大変な労力と時間が必要です。ご負担になる雪かき・除雪作業をお客様に代わって行います。",
    targetUrl: "",
    src: "https://placehold.jp/3d4070/ffffff/300x300.png",
    alt: "",
  },
});

const newsList = [
  {
    date: "2023.05.28",
    text: "ウェブサイトを公開しました。",
    targetUrl: "",
  },
];
</script>

<template>
  <div style="width: 100%">
    <div class="bg">
      <div
        style="
          background-color: rgb(236, 246, 249);
          text-align: left;
          width: 100%;
        "
      >
        下越地方のハウスクリーニングならクリーンプラス
      </div>
      <Header />
      <div style="height: 700px">
        <h1 style="text-align: left">
          車の内装クリーニングは<br />クリーンプラスに<br />おまかせください！
        </h1>
      </div>
      <!-- メインコンテンツ -->
      <div style="background-color: white">
        <div style="height: 100px"></div>
        <div class="news">
          <div class="news_title">NEWS</div>
          <div
            class="news_contents"
            v-for="(news, index) in newsList"
            :key="index"
          >
            <span>{{ news.date }}</span>
            <a :href="news.targetUrl">{{ news.text }}</a>
          </div>
        </div>

        <div style="height: 100px"></div>
        <!-- TODO: とりあえずCSSでどうにかするが、背景画像を用意したい -->
        <section class="about">
          <h2>
            快適な暮らしをご提供する<br />
            “クリーンプラス”の出張車内清掃
          </h2>
          <div>
            新潟県下越地方を中心に、地域に密着した車の内装クリーニングをはじめとしたサービスを提供しています。<br />
            当社では女性スタッフがおりますので、女性お一人の場合でも安心してご依頼いただけます。<br />
            丁寧な仕事と細やかなサービスにより、お客様のご要望にお応えしています。
          </div>
          <button type="button" class="btn btn-primary">店舗概要</button>
        </section>

        <section class="service">
          <div><h2>サービス一覧</h2></div>
          <div><CardLarge :card-info="card.car" /></div>
          <div class="card_list">
            <Card :card-info="card.extereor" />
            <Card :card-info="card.weeding" />
            <Card :card-info="card.window" />
            <Card :card-info="card.shoveling" />
          </div>
          <div class="banner">
            <img src="/madofuki.webp" class="banner" />
            <p class="banner_textline">
              <span class="banner_text--blue"
                >住宅・店舗等の室内清掃・片付け</span
              ><span class="banner_text">も承ります。</span>
              <span class="banner_subtext">view more</span>
            </p>
          </div>
        </section>

        <StoreInfo />

        <Contact />

        <Footer />
      </div>
    </div>
  </div>
</template>

<style scoped>
.bg {
  background-image: url(/top.webp);
  background-attachment: fixed;
  background-size: cover;
  background-position: center;
  text-align: center;
  margin: 0 calc(50% - 50vw);
  width: 100vw;
}

.news {
  border: 1px solid black;
  padding-top: 2rem;
  padding-bottom: 2rem;
  width: 90%;
  text-align: center;
  margin: 0 auto;
}

.news_title {
  display: inline-block;
  width: 30%;
}

.news_contents {
  display: inline-block;
  width: 70%;
}

.container {
  position: relative;
  background: #2c3e50;
  height: 50vh;
}

.about {
  background: rgb(124, 208, 208);
  margin: 0 auto;
}

.service {
  background: rgb(236, 246, 249);
}

.card_list {
  display: flex;
  justify-content: center;
}

.banner {
  position: relative;
  width: 800px;
  height: 300px;
  object-fit: cover;
  border: 1px solid rgb(149, 206, 216);
  border-radius: 5px;
  opacity: 0.75;
  margin: 0 auto;
}
.banner:hover {
  opacity: 0.5;
  transition: all 0.5s;
}

.banner_textline {
  position: absolute;
  top: 50%;
  /* left: 50%; */
  -ms-transform: translate(0%, -50%);
  -webkit-transform: translate(0%, -50%);
  transform: translate(0%, -50%);
  margin: 0;
  padding: 0;
  width: 100%;
  text-align: left;
}
.banner_text--blue {
  font-size: x-large;
  color: rgb(1, 153, 187);
}
.banner_text {
  font-size: x-large;
}
.banner_subtext {
  position: absolute;
  left: 80%;
}
</style>
