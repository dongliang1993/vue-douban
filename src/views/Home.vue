<template>
  <div class="home">
    <MyNav @showSearch="controlSearch"></MyNav>
    <Search></Search>
  </div>
</template>


<script>
  import MyNav from '@/components/Hello.vue'
  import Search from '@/views/Search'
  export default {
    name: 'home',
    components: {
      MyNav,
      Search
    },
    data () {
      return {
      }
    },
    methods: {
      controlSearch () {
        console.log(1)
      }
    }
  }
</script>

<style lang="scss" scope>

</style>
