<template>
  <div class="home">
    <Search @showSearch="controlSearch"></Search>
  </div>
</template>


<script>
  import Search from '@/components/Hello.vue'
  export default {
    name: 'home',
    components: {
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
