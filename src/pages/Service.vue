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

          <div id="exterior" class="service_card_wrapper">
            <div class="service_card">
              <h3>草取り・草刈り・除草剤の散布</h3>
              <hr class="service_card_hr" />
              <p>
                草が繁茂すると美観を損ねるだけでなく、周辺環境への影響も考慮しなければなりません。草取りサービスでは、プロのスタッフが丁寧に作業し、お庭や敷地内の草や雑草を根こそぎ取り除きます。
              </p>
              <p>
                また敷地が広い場合、雑草対策には、草刈りよりも除草剤を撒くことをおすすめします。草刈り・草取りに比べて作業時間が少なくできるため、費用を抑えることも可能です。
              </p>
              <div class="service_card_left"></div>
              <div class="service_card_right">
                <h4>草取り（手作業）</h4>
                <p>カマを使い草を手作業で取ります。</p>
                <p>
                  草の根から抜き取るため、再度雑草が生えてくるまでの時間が長くなります。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--tax">1㎡あたり</span
                  ><span class="service_card_value--amount">¥1,100</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>草刈り（草刈り機）</h4>
                <p>
                  草刈り機が入れる広さ、砂利が敷いていない場所等では、草刈りをおすすめします。広い敷地でも、時間をあまりかけずに、綺麗にする事が出来ます。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--tax">1㎡あたり</span
                  ><span class="service_card_value--amount">¥1,100</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>除草剤の散布</h4>
                <p>
                  除草剤を散布すると、今生えている雑草だけでなく飛来してくる雑草の種も発芽しないように処理することができます。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--tax">1㎡あたり</span
                  ><span class="service_card_value--amount">¥1,100</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
              </div>
            </div>
          </div>

          <div id="gutter" class="service_card_wrapper">
            <div class="service_card">
              <h3>側溝掃除・網戸の張替え</h3>
              <hr class="service_card_hr" />
              <div class="service_card_left"></div>
              <div class="service_card_right">
                <h4>側溝掃除</h4>
                <p>
                  側溝のふたを上げる作業は女性や高齢者にとって大変重労働です。当店はそのような側溝掃除のお手伝いをさせていただきます。
                </p>
                <p>なお、一人暮らしやお時間のない方からのご用命も承ります。</p>
                <p class="service_card_value">
                  <span class="service_card_value--tax">およそ10m</span
                  ><span class="service_card_value--amount">¥19,800</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>網戸の張替え</h4>
                <p>小さな穴は気づかないうちに大きく開いてしまいます。</p>
                <p>はやめの交換で虫の侵入を防ぎませんか？</p>
                <p class="service_card_value">
                  <span class="service_card_value--tax">高さ90㎝×幅90㎝</span
                  ><span class="service_card_value--amount">¥3,300</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <div class="service_card_note">
                  <p>※網戸の種類により変わります。</p>
                </div>
              </div>
            </div>
          </div>

          <div id="shoveling" class="service_card_wrapper">
            <div class="service_card">
              <h3>雪かき</h3>
              <hr class="service_card_hr" />
              <div class="service_card_left"></div>
              <div class="service_card_right">
                <p>
                  雪かきはどの家庭にとっても大変な作業です。時間に余裕の無い方、肉体労働が負担となる女性や高齢者の方など、自分で除雪をすることが困難な方にとって生活に大きな支障となる雪かき作業を、当店が承ります。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--tax">30分あたり</span
                  ><span class="service_card_value--amount">¥3,300</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
              </div>
            </div>
          </div>

          <div id="indoor" class="service_card_wrapper">
            <div class="service_card">
              <h3>住宅・店舗等の室内清掃・片付け</h3>
              <hr class="service_card_hr" />
              <p>
                ハウスクリーニング業者が使用する強力な溶剤は人体やペットに悪影響を及ぼします。
              </p>
              <p>
                当店はそのような強力な溶剤を使用せず、当店オリジナルのクリーナーを使い安全に配慮したスピーディな清掃を行います。
              </p>
              <div class="service_card_left"></div>
              <div class="service_card_right">
                <h4>浴室</h4>
                <p>
                  湿気によるカビや水アカ、皮脂汚れ、石鹸カスなど、それぞれの汚れに合った洗剤を使用しお掃除します。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>トイレ</h4>
                <p>
                  日頃のお掃除では落としきれない汚れ・カビ・黄ばみをキレイに洗浄し、除菌仕上げを行います。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>洗面台</h4>
                <p>
                  蛇口や細かな汚れやカビ・水アカ汚れなど、汚れの種類に適した洗剤を使用して、洗面器から鏡、蛇口までしっかりキレイにします。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>窓ガラス・サッシ・網戸の掃除</h4>
                <p>
                  砂埃、粉塵、タバコのヤニ等の汚れをプロの技術で美しく透明に磨き上げます。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500～</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>床・フローリングの掃除</h4>
                <p>
                  普段の掃除では取り切れない溜まってしまった床の汚れを、専用クリーナーでしっかり落とし、綺麗に仕上げます。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500～</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>カーペットやソファーの汚れ取り</h4>
                <p>
                  専用の機材、クリーナーを使用しシミ汚れや皮脂油、匂いを落とします。
                </p>
                <p class="service_card_value">
                  <span class="service_card_value--amount">¥5,500</span
                  ><span class="service_card_value--tax">(税込)</span>
                </p>
                <h4>住宅や事務所の片付け</h4>
                <p>お時間や内容により料金は変わります。</p>
                <p>お気軽にご相談ください</p>
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
