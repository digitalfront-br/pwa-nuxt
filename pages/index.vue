<template>
  <div>
    <BannerHome v-if="banners.edges" :dados="banners.edges" />
    <h1>home page</h1>
  </div>
</template>
<script>
import gql from 'graphql-tag'
export default {
  components: {
    BannerHome: () => import('@/components/BannerHome.vue')
  },
  data() {
    return {
      banners: []
    }
  },
  apollo:{
    banners: gql`
      query banners {
        banners {
          edges {
            node {
              id
              title
              content
              img:featuredImage {
                url:sourceUrl(size: LARGE)
              }
            }
          }
        }
      }`
  },
  mounted() {
    console.log('lista de banners ', this)
  }
}
</script>
