<template>
  <div style="height:100%">
      <my-header></my-header>
    <div class="container person">
        <div class="row">
            <!-- 主体部分 -->
            <div class="col-xs-16 main">
                <!-- 主体头 -->
                <div class="main-top">
                    <nuxt-link class="avatar" to="/u/123">
                        <img src="~/assets/img/default-avatar.jpg">
                    </nuxt-link>
                    <div class="title">
                        <nuxt-link class="name" to="/u/123">
                            测试用户
                        </nuxt-link>
                    </div>
                    <div class="info">
                        <ul>
                            <li>
                                <div class="meta-block">
                                    <nuxt-link to="/u/123/following">
                                        <p>12</p>
                                        关注
                                        <i class="fa fa-angle-right"></i>
                                    </nuxt-link>
                                </div>
                            </li>
                            <li>
                                <div class="meta-block">
                                    <nuxt-link to="/u/123/followers">
                                        <p>1</p>
                                        粉丝
                                        <i class="fa fa-angle-right"></i>
                                    </nuxt-link>
                                </div>
                            </li>
                            <li>
                                <div class="meta-block">
                                    <nuxt-link to="/u/123">
                                        <p>0</p>
                                        文章
                                        <i class="fa fa-angle-right"></i>
                                    </nuxt-link>
                                </div>
                            </li>
                            <li>
                                <div class="meta-block">
                                    <p>0</p>
                                    <div>字数</div>
                                </div>
                            </li>
                            <li>
                                <div class="meta-block">
                                    <p>0</p>
                                    <div>收获喜欢</div>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
                <!-- 主体内容 -->
                <div id="outer-container">
                    <ul class="trigger-menu">
                        <li>
                            <nuxt-link to="/u/123">
                                <i class="fa fa-book"></i>
                                文章
                            </nuxt-link>
                        </li>
                        <li class="active">
                            <nuxt-link to="/u/123/timeline">
                                <i class="fa fa-bell"></i>
                                动态
                            </nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/u/123">
                                <i class="fa fa-comments"></i>
                                最新评论
                            </nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/u/123">
                                <i class="fa fa-fire"></i>
                                热门
                            </nuxt-link>
                        </li>
                    </ul>
                    <div id="list-container">
                        <!-- 动态列表模块 -->
                        <ul class="note-list">
                            <!-- 关注了作者 -->
                            <li id="feed-123">
                                <div class="content">
                                    <div class="author">
                                        <nuxt-link class="avatar" to="/u/123">
                                            <img src="~/assets/img/default-avatar.jpg">
                                        </nuxt-link>
                                        <div class="info">
                                            <nuxt-link class="nickname" to="/u/123">测试用户</nuxt-link>
                                            <span>关注了作者 · 05.2 17:15</span>
                                        </div>
                                    </div>
                                    <div class="follow-detail">
                                        <div class="info">
                                            <nuxt-link class="avatar" to="/u/234">
                                                <img src="~/assets/img/follower.jpg">
                                            </nuxt-link>
                                            <a class="btn btn-default following">
                                                <i class="fa fa-check"></i>
                                                <span>已关注</span>
                                            </a>
                                            <nuxt-link class="title" to="/u/234">
                                                万里流水
                                            </nuxt-link>
                                            <p>写了 2437 字，被 22 人关注，获得了 117 个喜欢</p>
                                        </div>
                                        <div class="signature">
                                            简介：
张赞杰，笔名老牛，万里流水，广东省梅州市大埔县人，现在在广州东华职业学院就读物流管理，自小体弱多病，但是钟爱于写作，初中时学会写诗填词，至今已经作了大约有五百多首诗词。
                                        </div>
                                    </div>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <!-- 侧边栏 -->
            <div class="col-xs-7 col-xs-offset-1 aside">
                <div class="title">
                    个人介绍
                </div>
                <a class="function-btn" href="javascript:void(0)">
                    <i class="fa fa-pencil"></i>
                    编辑
                </a>
                <form style="display:none" action="/u/123" method="post"> 
                </form>
                <div class="description">
                    <div class="js-intro" style="display: block;">fasdfasdfasdf</div>
                </div>
                <ul class="list user-dynamic">
                    <li>
                        <nuxt-link to="/u/123/subscriptions">
                            <i class="fa fa-plus-square-o"></i>
                            <span>我关注的专题/文章/连载</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/u/123/liked notes">
                            <i class="fa fa-heart-o"></i>
                            <span>我喜欢的文章</span>
                        </nuxt-link>
                    </li>
                </ul>
                <!-- 专题和文集 -->
                <div>
                    <div class="title">我创建的专题</div>
                    <div class="new-collection-block">
                        <nuxt-link to="/collection/new" class="new-collection-btn">
                            <i class="fa fa-plus"></i>
                            <span>创建一个新专题</span>
                        </nuxt-link>
                    </div>
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
<style>
    .person .row{
        padding-top:30px ;
    }
    .person .main .main-top{
        margin-bottom: 20px;
    }
    .person .main .main-top .avatar{
        float: left;
        width: 80px;
        height: 80px;
        margin-left: -2px;
        display: block;
    }
    .person .main .main-top .title{
        padding: 5px 0 0 100px;
    }
    .person .main .main-top .title .name{
        display: inline-block;
        font-size: 21px;
        font-weight: 700;
        vertical-align: middle;
    }
    .person .main .main-top .info{
        margin-top: 5px;
        padding-left: 100px;
        font-size: 14px;
    }
    .person .main .main-top .info ul li{
        display: inline-block;
    }
    .person .main .main-top .info ul li .meta-block{
        font-size: 12px;
        margin: 0 7px 6px 0;
        padding: 0 7px 0 0;
        border-right: 1px solid #f0f0f0;
    }
    .person .main .main-top .info ul a{
        color: #969696;
    }
    .person .main .main-top .info ul p{
        margin-bottom: -3px;
        font-size: 15px;
        color: #333;
    }
    .person .main .main-top .info ul div{
        color: #969696;
    }
    .person .aside{
        padding: 0;
    }
    .person .aside .title{
        float: left;
        margin-bottom: 10px;
        font-size: 14px;
        color: #969696;
    }
    .person .aside .function-btn{
        float: right;
        font-size: 13px;
        color: #969696;
    }
    .person .aside form{
        margin-bottom: 20px;
    }
    .person .aside .description{
        position: relative;
        margin-bottom: 16px;
        padding: 0 0 16px;
        text-align: left;
        font-size: 0;
        border-bottom: 1px solid #f0f0f0;
        clear: both;
        word-break: break-word!important;
    
    }
    .person .aside .description .js-intro{
        margin-bottom: 10px;
        line-height: 20px;
        font-size: 14px;
    }
    .person .aside .user-dynamic{
        padding-bottom: 6px;
        margin-bottom: 16px;
        list-style: none;
        border-bottom: 1px solid #f0f0f0;
        clear: both;
    }
    .person .aside .user-dynamic li{
        margin-bottom: 10px;
    }
    .person .aside .user-dynamic li a{
        display: inline-block;
        font-size: 14px;
        color: #333;
        line-height: 30px;
    }
    .person .aside .user-dynamic li a i{
        margin-right: 10px;
        font-size: 20px;
        vertical-align: middle;
    }
    .person .aside .user-dynamic li a span{
        vertical-align: middle;
    }
    .person .aside .title{
        float: left;
        margin-bottom: 10px;
        font-size: 14px;
        color: #969696;
    }
    .person .aside .new-collection-block{
        position: relative;
        margin-bottom: 16px;
        padding: 0 0 16px;
        text-align: left;
        font-size: 0;
        border-bottom: 1px solid #f0f0f0;
        clear: both;
        word-break: break-word!important;
    }
    .person .aside .new-collection-block a{
        margin-right: 5px;
        font-size: 13px;
        color: #42c02e;
    }
    .person .aside .new-collection-btn i{
        padding-right: 2px;
    }
    .trigger-menu{
        margin-bottom: 20px;
        border-bottom: 1px solid #f0f0f0;
        list-style: none;
    }
    .trigger-menu li{
        position: relative;
        display: inline-block;
        padding: 8px 0;
        margin-bottom: -1px;
    }
    .trigger-menu li.active{
        border-bottom: 2px solid #646464;
    }
    .trigger-menu a{
        padding: 13px 20px;
        font-size: 15px;
        font-weight: 700;
        color: #969696;
        line-height: 25px;
    }
    .trigger-menu a i{
        margin-right: 5px;
        font-size: 17px;
    }
    .note-list li{
        position: relative;
        width: 100%;
        margin: 0 0 17px;
        padding: 0 2px 17px 0;
        border-bottom: 1px solid #f0f0f0;
        word-wrap: break-word;
    }
    .note-list .author{
        margin-bottom: 14px;
        font-size: 13px;
    }
    .note-list .author .avatar{
        display: inline-block;
        vertical-align: middle;
        margin: 0 5px 0 0;
        color: #333;
    }
    .note-list .author .info{
        display: inline-block;
        vertical-align: middle;
    }
    .note-list .author .info .nickname{
        vertical-align: middle;
    }
    .note-list .author .info span{
        display: inline-block;
        padding-left: 3px;
        color: #969696;
        vertical-align: middle;
    }
    .note-list .follow-detail{
        padding: 20px;
        background-color: hsla(0,0%,71%,.1);
        border: 1px solid #e1e1e1;
        border-radius: 4px;
        font-size: 12px;
    }
    .note-list .follow-detail .avatar{
        float: left;
        margin-right: 10px;
        width: 48px;
        height: 48px;
    }
    .note-list .follow-detail .btn{
        float: right;
        margin-top: 4px;
        padding: 8px 0;
        width: 100px;
    }
</style>

