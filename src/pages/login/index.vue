<template>
    <div class="login">
        <div class="head">
            <img src="@image/loginHead.png">
        </div>
        <div class="form">
            <div>
                <input type="text" placeholder="用户名">
            </div>
            <div>
                <input type="password" placeholder="密码">
            </div>
            <div style="margin-bottom: 5px">
                <input type="text" placeholder="请输入验证码">
            </div>
        </div>
        <div class="checkbox">
            <input type="checkbox" v-model="check"><span>记住密码</span>
        </div>
        <mt-button type="warning" class="my-button">default</mt-button>
    </div>
</template>
<script>
    export default {
        data() {
            return {
                check: true
            }
        }
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
                height: 2.5rem;
                margin: 1.25rem auto 1.25rem;
            }
        }
        .form{
            >div{
                height: 1.05rem;
                margin-bottom: 20px;
                input{
                    color: white;
                    box-sizing: border-box;
                    height: 100%;
                    border: 1px solid rgba(255,255,255,.3);
                    background: none;
                    border-radius: 1.875rem;
                    width: 90%;
                    font-size: .375rem;
                    padding-left: 1.25rem;
                }
            }
        }
        .checkbox{
            margin-bottom: 1.25rem;
            height: 1.05rem;
            line-height: 1.05rem;
            padding: 0 5%;
            text-align: left;
            input{
                vertical-align: middle;
                display: inline-block;
                height: .625rem;
                width: .625rem;
            }
            span{
                font-size: .375rem;
                color: white;
                vertical-align: middle;
                display: inline-block;
            }
        }
        .my-button{
            height: 1.05rem;
            width: 90%;
            border-radius: 1.875rem;
            background: linear-gradient(to right,#f8ce4c,#f3971f);
        }
    }
</style>


