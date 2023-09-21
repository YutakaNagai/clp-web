<script setup></script>

<template>
  <div class="footer_bg">
    <p><a>サイトマップ</a><a>お問い合わせ</a><a>プライバシーポリシー</a></p>
    <p>© Copyright © クリーンプラス All Rights Reserved.</p>
    <p>【掲載の記事・写真・イラストなどの無断複写・転載等を禁じます】</p>
  </div>
</template>

<style scoped>
.footer_bg {
  height: 200px;
  /* width: 100vw; */
  background-image: linear-gradient(
    90deg,
    rgba(4, 202, 255, 1),
    rgba(144, 245, 154, 1)
  );
  align-content: center;
  color: white;
  margin: 0 calc(50% - 50vw);
  padding: 0 calc(50vw - 50%);
  width: 100vw;
}
</style>
