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
      // parte main
      filters : [
        { text: 'Keywords'},
        { text: 'Location'},
        { text: 'All Categories', icon: 'fas fa-sort-down' },
        { text: 'Brand', icon: 'fas fa-sort-down' },
        { text: 'Fuel Type', icon: 'fas fa-sort-down' },
        { text: 'Transmission', icon: 'fas fa-sort-down' },
        { text: 'Status', icon: 'fas fa-sort-down' },
        { text: 'Search'}
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
      ],
      // campo input e bottone
      formInput: {
        fields: [
          {type: 'text', placeholder: 'Your Email Address'}
        ],
        button: {text: 'Subscribe'}
      } 
    };
  }
}

</script>

<template>
    
    <AppHeader :menuItems="menuItems"/>
  

  
    <AppMain :filters="filters" />
  

    
    <AppFooter :footerLists="footerLists" :formInput="formInput"/>
  
  
</template>

<style lang="scss">
@use './styles/generals.scss'



</style>
