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
            <router-link class="nav-link" :to="{ path: '/' }"
              >トップ</router-link
            >
          </li>
          <li class="nav-item">
            <router-link class="nav-link" :to="{ path: '/about' }"
              >店舗概要</router-link
            >
          </li>
          <li>
            <div class="nav-item dropdown">
              <a
                type="button"
                id="dropdown"
                class="nav-link dropdown-toggle"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >
                事業紹介
              </a>
              <ul class="dropdown-menu" aria-labelledby="dropdown">
                <li class="dropdown-item">
                  <router-link
                    class="nav-link"
                    :to="{ path: '/service', hash: '#service' }"
                    >サービス一覧</router-link
                  >
                </li>
                <li class="dropdown-item">
                  <router-link class="nav-link" :to="{ path: '/guide' }"
                    >ご利用の流れ</router-link
                  >
                </li>
              </ul>
            </div>
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
