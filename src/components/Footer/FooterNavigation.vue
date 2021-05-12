<template>
  <div class="col">
    <h3 class="footer__title">Navigation</h3>
    <ul class="footer__list">
      <li v-for="({ name, path }, i) in footerMenu" :key="i">
        <router-link :to="path" class="footer__link">
          {{ name }}
        </router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
   props: {
      footerMenu: {
         type: Array,
         required: true
      }
   }
}
</script>