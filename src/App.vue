<script>
// importo le componeneti
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


// utilizzo le componenti
export default {
  components : {
    AppHeader,
    AppMain,
    AppFooter
  },
  data () {
    return {
      // array per le voci della lista appheader
      menuItems: [
        { text: 'Home', href: '#'},
        { text: 'About Us', href: '#'},
        { text: 'Vehicles', href: '#'},
        { text: 'Dealers', href: '#'},
        { text: 'Packages', href: '#'},
        { text: 'Blog', href: '#'},
        { text: 'Contact', href: '#'},
      ],
      // footer lists
      footerLists : [
        {
          title: 'My Account',
          items: ['My Account', 'Checkout', 'Cart', 'Packages', 'Add Car']
        },
        {
          title: 'Quick Links',
          items: ['Home', 'About Us', 'Blog', 'Contacts', 'Refind & Returns']
        }
      ]
    };
  }
}

</script>

<template>
    <!-- ciclo la componenete  -->
    <AppHeader :menuItems="menuItems"/>
  

  
    <AppMain />
  

    <!-- ciclo la componenete -->
    <AppFooter :footerLists="footerLists"/>
  
  
</template>

<style lang="scss">
@use './styles/generals.scss'



</style>
