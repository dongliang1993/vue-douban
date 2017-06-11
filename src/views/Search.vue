<template>
  <div class="search">
    <div class="search-wrap">
      <span class="close-box">关1闭</span>
      <div class="input-box">
        <input type="text">
      </div>
    </div>
    <div class="recommend">
      <template v-for="item in recommendData">
        <div class="item-wrap">
          <div class="item-name">{{ item.name }}</div>
          <div class="item-subname">{{ item.subName }}</div>
        </div>
      </template>
    </div>
  </div>
</template>


<script>
  export default {
    name: 'search',
    components: {
    },
    data () {
      return {
        recommendData: [
          {name: '电影', subName: '影院热映', url: '1'},
          {name: '电视', subName: '影院热映', url: ''},
          {name: '图书', subName: '影院热映', url: ''},
          {name: '同城', subName: '影院热映', url: ''},
          {name: '小组', subName: '影院热映', url: ''},
          {name: '音乐', subName: '影院热映', url: ''},
          {name: '阅读', subName: '影院热映', url: ''},
          {name: '游戏', subName: '影院热映', url: ''},
          {name: '应用', subName: '影院热映', url: ''},
          {name: '东西', subName: '影s院热映', url: '1'},
          {name: 'FM', subName: '影院热映', url: ''},
          {name: '市集', subName: '影院热映', url: ''}
        ]
      }
    }
  }
</script>

<style lang="scss" scope>
.search {
  font-size: .14rem;

  .search-wrap {
    display: flex;
    height: .49rem;
    align-items: center;
    padding-left: .1rem;
    justify-content: space-around;
    border-bottom: 1px solid #ccc;

    .close-box {
      flex-grow: 1;
      text-align: center;
      color: #42bd56;
      font-size: .16rem;
    }
    .input-box {
      flex-grow:4;
      text-align: center;

      input {
        border: 0;
        background-size: .173rem;
        border-radius: 0.03rem;
        height: .32rem;
        font-size: .14rem;
        outline: none;
        width: 2.5rem;
        background: #ccc;
      }
    }
  }

  .recommend {
    display: flex;
    flex-wrap: wrap;
    .item-wrap {
      width: 1rem;
      text-align: center;
      flex-grow: 1;
      .item-name {
        font-size: .24rem;
        line-height: .28rem;
      }
      .item-subname {
        font-size: .12rem;
        color: #999;
      }
    }
  }
}
</style>
