<template>
  <div class="tabmusic">
    <div @click="recommendlink">
      <span class="iconfont icon-icon-test1"></span>
      <p>每日推荐</p>
    </div>
    <div @click="songslink">
      <span class="iconfont icon-icon-test2"></span>
      <p>歌单</p>
    </div>
    <div>
      <span class="iconfont icon-icon-test5"></span>
      <p>排行榜</p>
    </div>
    <div>
      <span class="iconfont icon-icon-test3"></span>
      <p>电台</p>
    </div>
    <div>
      <span class="iconfont icon-icon-test4"></span>
      <p>直播</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Tabmusic',
    data(){
      return {
        
      }
    },
    methods: {
      recommendlink(){
        this.$emit('recommendLink')
      },
      songslink(){
        this.$emit('songslink')
      }
    }
  }
</script>

<style scoped>
  .tabmusic {
    height: 100px;
    display: flex;
    border-bottom: 1px solid #f1f1f1;
  }
  .tabmusic div {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .tabmusic div span {
    font-size: 40px;
    color:#f52a1a;
    margin-bottom: 10px;
  }
  .tabmusic div p {
    color: #767676;
    font-weight: 500;
    font-size: 12px;
  }
</style>