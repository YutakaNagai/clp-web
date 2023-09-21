<script setup></script>

<template>
  <div class="contact_bg">
    <h2>お問い合わせ</h2>
    <p>〒956-0841 新潟県新潟市秋葉区東島51-3-2</p>
    <p class="contact_tel">TEL 090-1156-0010</p>
    <button type="button" class="btn btn-primary">お問い合わせはこちら</button>
  </div>
</template>

<style scoped>
.contact_bg {
  height: 400px;
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

.contact_tel {
  font-size: xxx-large;
}
</style>
