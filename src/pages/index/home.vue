<template>
  <div class="home">
    <common-header :showinput="false" :showback="false"></common-header>
    <div class="page-content">
        <ul>
          <li v-for="i in 30" :key="i">
            <div class="list-item" @click="todetail">
              <img src="@image/cqssc.png" alt="">
              <br>
              <span>重庆时时彩</span>
            </div>
          </li>
        </ul>
        <p class="banquan">版权所有 ©<span id="copyrightYear">2018</span></p>
    </div>
  </div>
</template>

<script>
import commonHeader from 'common/common-header'
export default {
  data () {
    return {
      num: 0
    }
  },
  created() {},
  methods: {
    todetail() {
      this.$router.togo('/Home/Detail')
    }
  },
  components: {
    commonHeader
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
@import "~styles/index.less";
@import "~styles/variable.less";
.home{
  ul{
    // margin: 4px 8px;
    padding: 10px 20px;
    background: white;
    list-style: none;
    display: inline-block;
    li{
      margin-top: 6px;
      float: left;
      width: calc(100% / 3);
      text-align: center;
      .list-item{
        padding: 10px 0;
        img{
          .h(120);
          .w(120);
        }
        span{
          .fs(26);
          color: #666;
        }
      }
    }
    clear: both;
  }
  .banquan{
    .fs(20);
    padding-bottom: 1.30666667rem;
  }
}
</style>
