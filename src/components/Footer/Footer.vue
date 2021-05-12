<template>
   <footer class="footer footer_bg">
      <div class="container">
         <div class="row">
            <FooterIcons />
            <FooterNavigation :footerMenu="footerMenu" />
            <FooterClient :footerMenuClient="footerMenuClient" />
            <FooterContacts />
         </div>
      </div>
   </footer>
</template>

<script>
import {menuList, menuClient} from '../../constants/menuLinks'
import FooterIcons from './FooterIcons'
import FooterNavigation from './FooterNavigation'
import FooterClient from './FooterClient'
import FooterContacts from './FooterContacts';
export default {
   data() {
      return {
         footerMenu: menuList,
         footerMenuClient: menuClient,
      }
   },
   components: {
      FooterIcons,
      FooterNavigation,
      FooterClient,
      FooterContacts
   },
}
</script>