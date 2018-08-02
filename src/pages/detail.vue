<template>
  <div class="game">
    <common-header :tittle="title" :showmore="true"></common-header>
    <div class="page-content">
      <div class="type">
        <span  @click="dialog">{{gameTitle}}<i></i></span>
        <div class="dialog" :class="{show: isShow}">
          <ul>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
            <li>fsd</li>
          </ul>  
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import commonHeader from 'common/common-header'
export default {
  data () {
    return {
      title: '重庆时时彩',
      gameTitle: '直选三',
      isShow: false
    }
  },
  components: {
    commonHeader
  },
  methods: {
    tohome () {
      this.$router.goBack()
    },
    dialog() {
      this.isShow = !this.isShow;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
@import "~styles/index.less";
@import "~styles/variable.less";
.game{
  .type{
    position: fixed;
    background: white;
    .fs(25);
    font-weight: 700;
    width: 100%;
    z-index: 111;
    color: #95948f;
    box-shadow: 0 6px 8px rgba(195,199,206,.4);
    span{
      display: block;
      position: relative;
      cursor: pointer;
      padding: 10px;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      i{
        &::after{
          border: 3px solid #c8c8cd;
          border-bottom-width: 0;
          border-left-width: 0;
          content: " ";
          top: 44%;
          right: 20px;
          position: absolute;
          width: 8px;
          height: 8px;
          -webkit-transform: translateY(-50%) rotate(45deg);
          transform: translateY(-50%) rotate(135deg);
        }
      }
    }
    .dialog{
      &.show{
        opacity: 1;
      }
      overflow-y: auto;
      opacity: 0;
      transition: opacity 1s;
      border-radius: 5px;
      background: white;
      z-index: 555;
      // top: 0;
      position: absolute;
      width: 100%;
      .h(300);
      box-shadow: 0 6px 8px rgba(195,199,206,.4);
    }
  }
}
</style>
