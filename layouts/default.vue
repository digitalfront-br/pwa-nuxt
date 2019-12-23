<template>
  <div>
    <Header />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
export default {
  components:{
    Header: () => import('@/components/Header.vue'),
    Footer: () => import('@/components/Footer.vue')
  }
}
</script>
