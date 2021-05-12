<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container">
      <a class="navbar-brand logo" href="/"
        ><img src="../assets/img/logo.png" alt="logo"
      /></a>
      <div
        class="collapse navbar-collapse collapse-fontsize"
        id="navbarSupportedContent"
      >
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li
            class="nav-item menu-link"
            v-for="({name, path}, index) in headerMenuList"
            :key="index"
          >
            <router-link
              class="nav-link active"
              aria-current="page"
              :to="path"
            >
              {{ name }}
            </router-link>
          </li>
        </ul>
        <div class="icons">
          <a href="https://www.facebook.com/" target="_blank"><img src="../assets/img/icons/f.png" alt="" /></a>
          <a href="https://www.pinterest.ru/" target="_blank"><img src="../assets/img/icons/p.png" alt="" /></a>
          <a href="https://www.instagram.com/" target="_blank"><img src="../assets/img/icons/inst.png" alt="" /></a>
          <a href="https://myaccount.google.com/" target="_blank"><img src="../assets/img/icons/g+.png" alt="" /></a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import {menuList} from '../constants/menuLinks'
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      headerMenuList: menuList,
    };
  },
};
</script>

<style lang="scss">
@import "../assets/layouts/index.scss";
.navbar {
  height: 90px;
}
.navbar-nav {
  height: 90px;
}
.logo {
  padding-right: 180px;
}
.collapse-fontsize {
  font-size: 18px;
}
.menu-link {
  padding: 25px 30px;

  &:hover {
    background: $grey;
  }
}
.icons {
  a {
    width: 30px;
    height: 30px;
    text-align: center;
    border: 1px solid $grey;
    border-radius: 50%;
    margin-right: 10px;
    display: inline-block;
  }
}
</style>