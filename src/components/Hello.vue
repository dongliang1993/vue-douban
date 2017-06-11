<template>
  <div class="nav">
    <div class="to-home">
      <router-link to="/index">豆瓣</router-link>
    </div>
    <ul class="nav-wrap">
     <li>
       <router-link to="/index" style="color: rgb(35, 132, 232);">电影</router-link>
     </li>
     <li>
       <router-link to="/index" style="color: rgb(159, 120, 96);">图书</router-link>
     </li>
     <li>
       <router-link to="/index" style="color: rgb(228, 168, 19);">广播</router-link>
     </li>
      <li>
        <router-link to="/index" style="color: rgb(42, 184, 204);">小组</router-link>
      </li>
    </ul>
    <span class="search" @click="showSearch">搜索</span>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
    }
  },
  methods: {
    showSearch () {
      this.$emit('showSearch')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.nav {
  display: flex;
  height: .48rem;
  font-size: .14rem;
  align-items: center;
  border-bottom: 1px solid #CCC;
  .to-home {
    flex-grow: 1;
    padding-left: .2rem;
    a {
      display: block;
      color: #00b600;
      line-height: .32rem;
      font-size: .22rem;
      font-weight: 600;
      height: .32rem;
      line-height:.32rem;
    }
  }
  .nav-wrap {
    flex-grow: 2;
    display: flex;
    margin: 0;
    padding: 0;

    list-style: none;
    li {
      flex: 1;
      margin: 0;
      padding: 0;
      text-align: center;
    }
  }

  .search {
    flex: 1;
  }
}

</style>
