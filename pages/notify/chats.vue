<template>
    <div style="height:100%">
        <my-header></my-header>
        <div class="container notify">
            <div class="row">
                <!-- 侧边栏 -->
              <my-aside></my-aside>   
                <!-- 主题部分 -->
                <div class="col-xs-16 col-xs-offset-8 main">
                    <div>
                        <div class="menu">全部简信</div>
                        <ul class="jianxin-list">
                            <li>
                                <div class="pull-right">
                                    <span class="time">04.20 15:36</span>
                                    <div class="open">
                                        <a href="javascript:void(0);">
                                            <i class="fa fa-angle-down"></i>
                                        </a>
                                        <!-- <ul class="dropdown-menu">
                                            <li>
                                                <a><i class="fa fa-trash-o">删除会话</i></a>
                                            </li>
                                            <li>
                                                <a><i class="fa fa-ban">加入黑名单</i></a>
                                            </li>
                                            <li>
                                                <a><i class="fa fa-flag-o">举报用户</i></a>
                                            </li>
                                        </ul> -->
                                    </div>
                                    <nuxt-link to="/u/123" class="avatar">
                                        <img src="~/assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <nuxt-link to="/u/123" class="name">
                                        简宝玉
                                    </nuxt-link>
                                    <nuxt-link to="/notify/chats/123" class="wrap"> 
                                        <p> 欢迎加入丰富多彩的原创内容社区—简书。新手有关简书的任何疑问请点击链接查看 http://w...</p>
                                    </nuxt-link>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    import myHeader from "~/components/myHeader"
    import myAside from "~/components/myAside"
    export default {
    components: {
        myHeader,
        myAside

    },
    data() {
        return {
        };
    }    
};
</script>

<style scoped>
    .notify .row{
        padding: 30px 0;
        overflow: hidden;
    }
    .notify .row::after{
        content: "";
        clear: both;
    }
    .main{
        padding-left: 0;
    }
    .main .menu{
        margin-bottom: 20px;
        font-size: 14px;
        font-weight: 700;
    }
    .main .jianxin-list li{
        position: relative;
        border-top: 1px solid #f0f0f0;
    }
    .main .jianxin-list li .pull-right{
        margin: 20px 20px 0 0;
        font-size: 13px;
        float: right !important;
    }
    .main .jianxin-list li .pull-right .time{
        color: #9b9b9b;
    }
    .main .jianxin-list li .pull-right div{
        display: inline-block;
    }
    .main .jianxin-list li .pull-right div i{
        color: #9b9b9b;
    }
    /* .main .jianxin-list li .pull-right .dropdown-menu{
        top: auto;
        left: auto;
        right: 15px;
        color: #333;
        min-width: inherit;
        position: absolute;
        z-index: 1000;
        float: left;
        padding: 5px 0;
        margin: 2px 0 0;
        font-size: 14px;
        text-align: left;
        background-color: #fff;
        border: 1px solid rgba(0,0,0,.15);
        border-radius: 4px;
        background-clip: padding-box;
    }
    .main .jianxin-list li .pull-right .dropdown-menu li{
        border: none!important;
    }
    .main .jianxin-list li .pull-right .dropdown-menu li a{
        padding: 10px 20px;
        display: block;
        clear: both;
        font-weight: 400;
        line-height: 1.42857;
        color: #333;
        white-space: nowrap;
    } */
    .main .jianxin-list .avatar{
        float: left;
        margin: 20px 10px 20px 20px;
        width: 48px;
        height: 48px;
        display: block;
    }
    .main .jianxin-list .name{
        position: absolute;
        top: 25px;
        font-size: 15px;
    }
    .main .jianxin-list .wrap{
        display: block;
        padding: 20px 20px 20px 0;
        min-height: 88px;
    }
    .main .jianxin-list .wrap p{
        margin: 28px 0 0;
        font-size: 12px;
        color: #999;
        overflow: hidden;
        text-overflow: ellipsis;
        white-space: nowrap;
    }
</style>
