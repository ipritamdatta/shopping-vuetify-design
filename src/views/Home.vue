<template>
  <div>
      <Header />
      <PopularProducts/>
      <Footer />
  </div>
</template>

<script>
import Header from '../components/home/Header.vue'
import Footer from '../components/home/Footer.vue'
import PopularProducts from '../components/home/PopularProducts.vue'

export default {
    components:{
      Header,
      Footer,
      PopularProducts
    }
}
</script>