<script setup>
import { ref } from "vue";
import Header from "../components/Header.vue";
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
        <h1 style="text-align: left">事業紹介</h1>
        <p>SERVICE</p>
      </div>
      <!-- メインコンテンツ -->
      <div>
        <section id="service" class="service">
          <div><h2>サービス一覧</h2></div>
          <div class="service_anchorList">
            <ul>
              <li><a href="#cleaning">車の内装クリーニング・洗車</a></li>
              <li><a href="#exterior">エクステリア掃除</a></li>
              <li><a href="#weeding">草取り</a></li>
              <li><a href="#gutter">側溝掃除・網戸の張り替え</a></li>
              <li><a href="#shoveling">雪かき</a></li>
              <li><a href="#indoor">住宅・店舗等の室内清掃・片付け</a></li>
            </ul>
          </div>

          <div id="cleaning" class="service_card_wrapper">
            <div class="service_card">
              <h3>車の内装クリーニング・洗車</h3>
              <hr class="service_card_hr" />
              <div class="service_card_left"></div>
              <div class="service_card_right">
                <h4>内装・クリーニング</h4>
                <p>
                  素材・汚れに応じた機材・液剤等を使用し車内の隅々まで丁寧にクリーニングいたします。
                </p>
                <p>
                  お子様やペットへの影響を考えお客様の要望に応じて、スチームでの消毒も行っております。
                </p>
                <table class="service_card_table">
                  <tr>
                    <td>軽自動車</td>
                    <td>22,000円（税込）</td>
                  </tr>
                  <tr>
                    <td>小型車（5人乗り）</td>
                    <td>27,500円（税込）</td>
                  </tr>
                  <tr>
                    <td>普通車（5人乗り）</td>
                    <td>33,000円（税込）</td>
                  </tr>
                  <tr>
                    <td>ミニバン（6人乗り以上）小型</td>
                    <td>38,500円（税込）</td>
                  </tr>
                  <tr>
                    <td>ミニバン（6人乗り以上）大型</td>
                    <td>49,500円（税込）</td>
                  </tr>
                  <tr>
                    <td>SUV 小型</td>
                    <td>33,000円（税込）</td>
                  </tr>
                  <tr>
                    <td>SUV 大型</td>
                    <td>38,500円（税込）</td>
                  </tr>
                </table>
                <div class="service_card_note">
                  <p>※バン・トラックなどはご相談ください。</p>
                  <p>
                    ※店舗や住宅のソファーや、ベビーシートなどもご相談ください。
                  </p>
                </div>
                <h4>洗車（外装のみ）</h4>
                <p>
                  たっぷりの水を使用して、手洗いにこだわり丁寧に洗いあげます。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>洗車（外装＋ワックスがけ）</h4>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥11,000</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>ガラス撥水加工</h4>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>ヘッドライトクリーニング</h4>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>タイヤ交換</h4>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>オイル交換</h4>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <div class="service_card_point_box">
                  <p class="service_card_point_title">Point</p>
                  <ul>
                    <li class="service_card_point_text">
                      業者に2〜3日預けていた→<span
                        class="service_card_point_text--bold"
                        >当店はおよそ3時間。ご自宅で時間を有効に使えます。</span
                      >
                    </li>
                    <li class="service_card_point_text">
                      施工状況を確認できなかった→<span
                        class="service_card_point_text--bold"
                        >目の前で施工が見えるので安心</span
                      >
                    </li>
                    <li class="service_card_point_text">
                      業者に任せっきりだった→<span
                        class="service_card_point_text--bold"
                        >細かい注文にも対応</span
                      >
                    </li>
                    <li class="service_card_point_text">
                      高額な料金→<span class="service_card_point_text--bold"
                        >リーズナブルな料金設定</span
                      >
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>

          <div id="exterior" class="service_card_wrapper">
            <div class="service_card">
              <h3>エクステリア掃除</h3>
              <hr class="service_card_hr" />
              <div class="service_card_left"></div>
              <div class="service_card_right">
                <h4>エクステリア掃除</h4>
                <p>
                  コンクリート壁や玄関アプローチは雨風や排気ガスによって黒ずみや苔が付着し、経年劣化が進みます。
                </p>
                <p>
                  掃除を行うことで汚れやカビ、藻などを徹底的に取り除き、外壁の耐久性を保ちながら美観を向上させます。
                </p>
                <p>汚れの除去を通じて塗料やタイルの耐久性も向上します。</p>
                <p>早めの清掃により、トータルコストの削減も図れます。</p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥1,100</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <div class="service_card_note">
                  <p>※薬品使用で1㎡あたり¥200プラスとなります。</p>
                  <p>※駐車スペース１台分（約5m×2.5m）およそ￥10,000</p>
                </div>
              </div>
            </div>
          </div>
        </section>

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
  margin: 0 auto;
}

.service_anchorList {
  margin: 0 auto;
}

.service_card_wrapper {
  padding: 25px;
}

.service_card {
  background: white;
  border-radius: 20px;
  box-shadow: 5px 10px 20px rgba(0, 0, 0, 0.25);
  width: 80%;
  margin: 0 auto;
  padding: 50px;
  margin-bottom: 100px;
}

.service_card_hr {
  width: 90%;
}

.service_card_left {
  width: 30%;
  margin-left: 0;
  margin-right: auto;
}

.service_card_right {
  width: 70%;
  margin-left: auto;
  margin-right: 0;
  text-align: left;
}

.service_card_table {
  width: 100%;
}
.service_card_table tr:nth-child(odd) td {
  background-color: rgb(236, 246, 249);
}

.service_card_note {
  margin-right: 0;
  margin-left: auto;
  text-align: right;
  font-size: small;
}

.service_card_value {
  text-align: right;
}
.service_card_value--amount {
  font-size: xx-large;
  font-weight: bold;
}

.service_card_value--tax {
  font-size: large;
  font-weight: bold;
}

.service_card_point_box {
  border: 5px solid rgb(120, 200, 219);
}

.service_card_point_title {
  color: rgb(1, 153, 187);
  font-size: x-large;
  font-weight: bold;
}

.service_card_point_text {
}

.service_card_point_text--bold {
  color: rgb(1, 153, 187);
  font-size: large;
  font-weight: bold;
}
</style>
