<template>
  <div>
    <Header />
    <nuxt />
    <Footer />
    <Mobile />
  </div>
</template>

<script>
export default {
  components:{
    Header: () => import('@/components/Header.vue'),
    Footer: () => import('@/components/Footer.vue'),
    Mobile: () => import('@/components/Mobile.vue')
  }
}
</script>
