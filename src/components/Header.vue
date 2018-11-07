<template>
  <div class="header">
    <div class="header-left">
        <span class="iconfont">&#xe624;</span>
    </div>
    <div class="header-input">
        <span class="iconfont">&#xe632;</span>输入城市景点/游玩主题
    </div>
    <div class="header-right">城市<span class="iconfont">&#xe64a;</span></div>
  </div>
</template>

<script>
import '../assets/styles/varibles.css'
export default {
  name : 'HomeHeader'
}
</script>

<style scoped>
  .header{
      width: 100%;
      display: flex;
      background: var(--bgColor);
      color: #fff;
      line-height: 64px;
  }
  .header-left{
      width : 48px;
      float: left;
      text-align: center;
  }
  .header-input{
      flex: 1;
      height: 40px;
      background: #fff;
      border-radius: 8px;
      margin-top: 12px;
      margin-left: 4px;
      padding-left: 4px;
      color: #ccc;
      line-height: 40px;
  }
  .header-right{
      width: 64px;
      float: right;
      text-align: center;
  }
</style>
