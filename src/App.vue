<template>
    <TheHeader />
    <TheSearch />
    <TheCategories />
    <TheBanners />
    <TheContent />
    <TheFooter />
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheSearch from './components/TheSearch.vue'
import TheCategories from './components/TheCategories.vue'
import TheBanners from './components/TheBanners.vue'
import TheContent from './components/TheContent.vue'
import TheFooter from './components/TheFooter.vue'

export default {
  components: {
    TheHeader,
    TheSearch,
    TheCategories,
    TheBanners,
    TheContent,
    TheFooter
  }
}
</script>