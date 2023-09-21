<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <nav class="navbar bg-white navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <img src="/logo.svg" alt="Bootstrap" width="300" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div
        class="collapse navbar-collapse d-flex justify-content-end"
        id="navbarNavDropdown"
        style="margin: 0 0 0 auto"
      >
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">トップ</a>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" :to="{ path: '/about' }"
              >店舗概要</router-link
            >
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              事業紹介
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">サービス一覧</a></li>
              <li><a class="dropdown-item" href="#">ご利用の流れ</a></li>
            </ul>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">検索</a>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-primary">お問い合わせ</button>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.logo {
  width: 300px;
  height: 37.5px;
}
</style>
