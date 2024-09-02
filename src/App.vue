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

      vehicles: [
        { title: 'Cabrio', image: '/img/cabrio.jpg', listings: '3' },
        { title: 'Coupe', image: '/img/coupe.jpg', listings: '0' },
        { title: 'Hatchback', image: '/img/hatchback.jpg', listings: '2' },
        { title: 'Pick Up', image: '/img/pickup.jpg', listings: '0' },
        { title: 'Sedan', image: '/img/sedan.jpg', listings: '3' },
        { title: 'Suv', image: '/img/suv.jpg', listings: '4' }
      ],

      cards: [
      { model: 'BMW M9', type: 'Cabrio', image: '/img/bmw-8-series-convertible.jpg', price: '34,000', brand: 'BMW', fuel: 'Electric' },
      { model: 'BMW M8', type: 'Cabrio', image: '/img/bmwimage2.jpg', price: '34,000', brand: 'BMW', fuel: 'Diesel' },
      { model: 'BMW M4', type: 'Cabrio', image: '/img/bmwimage3.jpg', price: '34,000', brand: 'BMW', fuel: 'Gasoline' },
      { model: 'Seat Ibiza', type: 'Hatchback', image: '/img/seat1.jpg', price: '27,000', brand: 'Seat', fuel: 'Electric' },
      { model: 'Seat Arona', type: 'SUV', image: '/img/seat2.jpg', price: '68,000', brand: 'Seat', fuel: 'Gasoline' },
      { model: 'Volswagen Taigo', type: 'SUV', image: '/img/vw-1.jpg', price: '52,000', brand: 'Volswagen', fuel: 'Electric' },
      { model: 'Volswagen T-Cross', type: 'SUV', image: '/img/vw-2.jpg', price: '47,000', brand: 'Volswagen', fuel: 'Diesel' },
      { model: 'Volswagen Passat', type: 'Sedan', image: '/img/vw-3.jpg', price: '32,000', brand: 'Volswagen', fuel: 'Diesel' }
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
  

  
    <AppMain :filters="filters" :vehicles="vehicles" :cards="cards"/>
  

    
    <AppFooter :footerLists="footerLists" :formInput="formInput"/>
  
  
</template>

<style lang="scss">
@use './styles/generals.scss'



</style>
