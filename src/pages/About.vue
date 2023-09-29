<script setup>
import { ref } from "vue";
import Header from "../components/Header.vue";
import StoreInfo from "../components/StoreInfo.vue";
import Contact from "../components/Contact.vue";
import Footer from "../components/Footer.vue";
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
      <div style="height: 200px">
        <h1 style="text-align: left">店舗概要</h1>
        <p>ABOUT</p>
      </div>
      <!-- メインコンテンツ -->
      <div style="background-color: white">
        <section class="service">
          <div><h2>ごあいさつ</h2></div>
          <div>
            <div><img src="/goaisatsu.webp" /></div>
            <div>
              <p>
                私たちの会社では、女性目線での細やかなサービスを心掛けております。お客様のご要望やご相談には、どんな小さなことでも丁寧にお応えさせていただきます。お住まいやお車に関するお悩みやご希望がございましたら、お気軽にお申し付けください。私たちが心を込めてサポートいたします。
              </p>
              <p>
                私たちの目標は、お客様が安心して暮らせる環境を提供することです。それはきめ細かなサービスと、お客様との信頼関係を築くことによって成り立ちます。私たちはいつもお客様の満足度を最優先に考え、ご期待に応えるために努力し続けます。ご要望やご意見に対しても、真摯に向き合い改善に努めます。
              </p>
              <p>
                私たちが提供するサービスがお客様の生活の一部となり、より良い日常をサポートできることを願っております。
              </p>
            </div>
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
  background-image: url(/juutaku.webp);
  background-attachment: fixed;
  background-size: cover;
  background-position: center;
  text-align: center;
  margin: 0 calc(50% - 50vw);
  width: 100vw;
}

.service {
  background: rgb(236, 246, 249);
}
</style>
