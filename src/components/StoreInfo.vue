<script setup></script>

<template>
  <section class="store">
    <div><h2>店舗概要</h2></div>
    <div class="store_contents">
      <div>
        <table>
          <tr class="store_table">
            <td class="store_table_left">店舗名</td>
            <td class="store_table_right">クリーンプラス</td>
          </tr>
          <tr class="store_table">
            <td class="store_table_left">代表</td>
            <td class="store_table_right">永井 敏子</td>
          </tr>
          <tr class="store_table">
            <td class="store_table_left">所在地</td>
            <td class="store_table_right">
              〒956-0841 新潟県新潟市秋葉区東島51-3-2
            </td>
          </tr>
          <tr class="store_table">
            <td class="store_table_left">電話番号</td>
            <td class="store_table_right">090-1156-0010</td>
          </tr>
        </table>
      </div>
      <div class="store_map">Map</div>
    </div>
  </section>
</template>

<style scoped>
.logo {
  width: 300px;
  height: 37.5px;
}

.store {
  position: relative;
  width: 90%;
  margin: 0 auto;
}
.store_contents {
  display: flex;
  justify-content: space-around;
}

.store_table {
  text-align: left;
  border-color: black;
  border-style: solid;
  border-width: 1px 0;
  font-size: large;
}
.store_table_left {
  width: 20%;
  white-space: nowrap;
}
.store_table_right {
  width: 80%;
  white-space: nowrap;
}
.store_map {
  border: 1px solid black;
  width: 500px;
  height: 500px;
}
</style>
