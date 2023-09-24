<template>
  
  <div>
    <CustomNavBar/>
    <SearchBar/>
    <CardsProfessores/>
    <CustomFooter/>
  </div>
</template>

<script>
import  CustomFooter from '../components/CustomFooter.vue'
import  CustomNavBar from '../components/CustomNavBar.vue'
import CardsProfessores from '../components/home/CardsProfessores.vue'
import SearchBar from '../components/home/SearchBar.vue'

export default {
    name:'HomeView',
  components: {
    CustomNavBar,
    CustomFooter,
    SearchBar,
    CardsProfessores,
  }
}
</script>

<style>

</style>