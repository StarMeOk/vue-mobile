<template>
    <div class="login">
        <div class="head">
            <img src="@image/loginHead.png">
        </div>
        <div class="form">
            <div class="username">
                <input type="text" placeholder="用户名">
            </div>
            <div class="username">
                <input type="text" placeholder="密码">
            </div>
            <div class="username">
                <input type="text" placeholder="请输入验证码">
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        
    }
</script>
<style lang="less" scoped>
    @import "~styles/index.less";
    @import "~styles/variable.less";
    .login{
        height: 100%;
        width: 100%;
        background: linear-gradient(#202643,#262c49,#202643) !important;
        .head{
            img{
                .h(200);
                margin: 0 auto;
                .mt(100);
                .mb(50);
            }
        }
        .form{
            >div{
                margin: 6px 0;
                .fs(14);
                .lh(20);
                input{
                    width: calc(100% - 0.66666rem);
                    border: 1px solid rgba(255,255,255,.3);
                    padding: 12px 10px 12px 38px;
                }
            }
        }
    }
</style>


