<template>
  <div id="app">
    <div class="container-full">
    <b-navbar toggleable type="inverse" variant="info" sticky>
      <b-nav-toggle target="nav_collapse"></b-nav-toggle>

      <b-link class="navbar-brand" to="#">
        <span>Bang!</span>
      </b-link>

      <b-collapse is-nav id="nav_collapse">
        <b-nav is-nav-bar>
          <b-nav-item-dropdown text="遊戲牌" right disabled>
          <b-dropdown-item>全部</b-dropdown-item>
          <b-dropdown-item>藍邊牌</b-dropdown-item>
          <b-dropdown-item>棕邊牌</b-dropdown-item>
          <b-dropdown-item>綠邊牌</b-dropdown-item>
        </b-nav-item-dropdown>
        </b-nav>
      </b-collapse>
    </b-navbar>
    <router-view></router-view>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
@import '~bootstrap/dist/css/bootstrap.css';
@import '~bootstrap-vue/dist/bootstrap-vue.css';
</style>
