<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item" v-for="(menu, index) in headerMenuList" :key="index">
            <router-link class="nav-link active" aria-current="page" :to="menu.path">
              {{ menu.name }}
            </router-link>
          </li>
        </ul>
        <div>
          <a href="#"><img src="../assets/img/icons/f.png" alt=""></a>
          <a href="#"><img src="../assets/img/icons/p.png" alt=""></a>
          <a href="#"><img src="../assets/img/icons/inst.png" alt=""></a>
          <a href="#"><img src="../assets/img/icons/g+.png" alt=""></a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      headerMenuList: [
        {name: 'Home', path: '/'},
        {name: 'About Us', path: '/about'},
        {name: 'Property', path: '/property'},
        {name: 'Our Blog', path: '/blog'},
        {name: 'Contacts', path: '/contacts'},
      ]
    }
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
