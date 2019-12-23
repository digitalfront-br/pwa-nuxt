<template>
  <div>
    <BannerHome />
    <h1>home page</h1>
  </div>
</template>
<script>
export default {
  components: {
    BannerHome: () => import('@/components/BannerHome.vue')
  }
}
</script>
