<template>
  <div style="height:100%">
      <my-header></my-header>
      <div class="container follow">
          <div class="row">
              <!-- 侧边栏 -->
              <div class="aside">
                  <a class="change-type">
                      全部关注
                      <i class="fa fa-toggle-down"></i>
                  </a>
                  <ul class="dropdown-menu arrow-top">
                      <li><a>全部关注</a></li>
                      <li><a>只看作者</a></li>
                      <li><a>只看专题</a></li>
                      <li><a>只看文集</a></li>
                      <li><a>只看推送更新</a></li>
                  </ul>
                  <nuxt-link to="/recommendation" class="add-people">
                        <i class="fa fa-user-plus"></i>
                        <span>添加关注</span>
                  </nuxt-link>
                  <ul class="js-follow-list">
                      <li class="active">
                          <nuxt-link to="/timeline" class="wrap">
                            <div class="avatar">
                                <img src="~/assets/img/jianyouquan.png">
                            </div>
                            <div class="name">
                                简友圈
                            </div>
                          </nuxt-link>
                      </li>
                      <li>
                          <nuxt-link to="/123/collection" class="wrap">
                            <div class="avatar-collection">
                                <img src="~/assets/img/default-avatar.jpg">
                            </div>
                            <div class="name">古风客栈</div>
                            <span class="count">1</span>
                          </nuxt-link>
                      </li>
                      <li>
                          <nuxt-link to="/123/collection" class="wrap">
                            <div class="avatar-collection">
                                <img src="~/assets/img/default-avatar.jpg">
                            </div>
                            <div class="name">连载小说</div>
                          </nuxt-link>
                      </li>
                      <li>
                          <nuxt-link to="/123/collection" class="wrap">
                            <div class="avatar-collection">
                                <img src="~/assets/img/default-avatar.jpg">
                            </div>
                            <div class="name">程序员</div>
                          </nuxt-link>
                      </li>
                      <li>
                          <nuxt-link to="/123/collection" class="wrap">
                            <div class="avatar">
                                <img src="~/assets/img/default-avatar.jpg">
                            </div>
                            <div class="name">牛客网</div>
                          </nuxt-link>
                      </li>
                  </ul>
              </div>
              <!-- 文章列表 -->
              <div class="col-xs-16 col-xs-offset-8 main">
                  <div>
                      <ul class="note-list">
                          <li class="have-img">
                              <nuxt-link to="/p/123" class="wrap-img">
                                  <img src="~/assets/img/note1.jpg">
                              </nuxt-link>
                              <div class="content">
                                  <div class="author">
                                    <nuxt-link to="/u/123" class="avatar">
                                        <img src="~/assets/img/default-avatar.jpg">
                                    </nuxt-link>
                                    <div class="info">
                                        <nuxt-link to="/u/123" class="nickname">
                                            枫拾贰
                                        </nuxt-link>
                                        <span>喜欢了文章 · 1小时前</span>
                                    </div>
                                  </div>
                                  <nuxt-link to="/p/123" class="title">
                                成长征文|等了那么多年，只为再次遇见你
                              </nuxt-link>
                              <p class="abstract">2018/5/2  星期三  晴 你来，我热情欢迎。你走，我也不遗憾。  “小枫，看什么呢?快点走了。”  我的同桌边说着边向我眼前摆摆手，好像一种很不耐烦的样子，大抵是她见...</p>
                              <div class="meta">
                                    <div class="origin-author">
                                      <nuxt-link to="/u/123">
                                        边瑶姑娘
                                      </nuxt-link>
                                    </div>
                                    <nuxt-link to="/p/123">
                                        <i class="fa fa-eye"></i>
                                            1500
                                    </nuxt-link>
                                    <nuxt-link to="/p/123">
                                        <i class="fa fa-comment"></i>
                                            100
                                    </nuxt-link>
                                        <span>
                                            <i class="fa fa-heart"></i>
                                                20
                                        </span>
                                </div>
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
import myHeader from "../components/myHeader";
export default {
  head: {
    title: "关注-简书",
    meta: [
      { charset: "utf-8" },
      { name: "keywords", content: "简书关注页" },
      { name: "description", content: "简书关注页" },
      { name: "author", content: "wwj" }
    ]
  },
  components: {
    myHeader
  },
  data() {
    return {
      name: "关注页"
    };
  }
};
</script>

<style scoped>
    /******************关注页布局开始*****************************/
.follow .aside{
    position: fixed;
    top: 0;
    bottom: 0;
    margin: 86px 0 0;
    padding: 0 0 30px;
    width: 280px;
    overflow: auto;
    border-right: 1px solid #f0f0f0;
}
.follow .aside .change-type{
    margin-left: 15px;
    font-size: 15px;
}
.follow .aside .change-type i{
    margin-left: 5px;
    color: #c8c8c8;
}
.follow .aside ul{
    margin-top: 7px;
    list-style: none;
    border-top: 1px solid #f0f0f0;
}
.follow .aside .dropdown-menu{
    top: 23px;
    left: 20px;
    min-width: 130px;
    text-align: center;
    border-color: transparent;
    box-shadow: 0 2px 8px rgba(0,0,0,.1);
    position: absolute;
    z-index: 1000;
    float: left;
    padding: 5px 0;
    margin: 2px 0 0;
    font-size: 14px;
    background-color: #fff;
    border: 1px solid rgba(0,0,0,.15);
    border-radius: 4px;
    background-clip: padding-box;
    display: none;
}
.follow .aside .dropdown-menu li{
    line-height: 20px;   
}
.follow .aside .dropdown-menu li:hover{
    background-color: #f5f5f5;
}
.follow .aside .dropdown-menu li a{
    padding: 10px 20px;
    display: block;
    clear: both;
    font-weight: 400;
    line-height: 1.42857;
    color: #333;
    white-space: nowrap;
    
}

.follow .aside .add-people{
    float: right;
    margin: 4px 10px 0 0;
    font-size: 13px;
    color: #333;
}
.follow .aside .add-people span{
    margin-left: 4px;
}
.follow .aside .js-follow-list{
    margin-top: 7px;
    list-style: none;
    border-top: 1px solid #f0f0f0;
}
.follow .aside .js-follow-list li{
    line-height: 20px;
}
.follow .aside .js-follow-list li .wrap{
    padding: 10px 13px;
    display: block;
}
.follow .aside .js-follow-list li .wrap:hover{
    background-color: #f0f0f0;
}
.follow .aside .js-follow-list li .wrap .avatar{
    width: 40px;
    height: 40px;
    margin-right: 4px;
    display: inline-block;
}
.follow .aside .js-follow-list li .wrap .avatar img{
    width: 100%;
    height: 100%;
    border-radius: 50%;
}
.follow .aside .js-follow-list li .wrap .name{
    font-size: 14px;
    padding: 10px 13px;
    display: block;
    display: inline-block;
    max-width: 160px;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
}
.follow .aside .js-follow-list li .wrap .avatar-collection{
    width: 40px;
    height: 40px;
    margin-right: 4px;
    display: inline-block;
}
.follow .aside .js-follow-list li .wrap .avatar-collection img{
    width: 100%;
    height: 100%;
    border: 1px solid #ddd;
    border-radius: 10%;
}
.follow .aside .js-follow-list li .wrap span{
    float: right;
    margin-top: 10px;
    font-size: 14px;
    color: #969696;
}
.note-list li {
    position:relative;
    width:100%;
    padding:0 0 17px;
    margin:0 0 17px;
    border-bottom:1px solid #f0f0f0;
}
.note-list li .wrap-img {
    position: absolute;
    top: 50%;
    margin-top: -68px;
    right: 0;
    width: 150px;
    height: 120px;
}
.note-list li .wrap-img img{
    width: 100%;
    height: 100%;
    border-radius: 4px;
    border: 1px solid #f0f0f0;
}
.note-list li.have-img>div {
    padding-right:160px;
}
.note-list .author {
    font-size:13px;
    margin-bottom:14px;
    vertical-align: middle;
}
.note-list .author .avatar {
    display:inline-block;
    width:32px;
    height:32px;
    margin-right:5px;
    vertical-align: middle;
}
.avatar img {
    max-width:100%;
    height:auto;
    display:inline-block;
    border-radius: 50%;
    border:1xp solid #ddd;
}
.note-list .author .info {
    display:inline-block;
    vertical-align: middle;
}
.note-list .author .nickname {
    vertical-align: middle;
}
.note-list .author .time {
    color:#969696;
    vertical-align: middle;
    padding-left:5px;
}
.note-list .title {
    display:block;
    margin:-7px 0 4px;
    font-size:18px;
    line-height:1.5;
    font-weight: 700;
}
.note-list .title:hover {
    text-decoration: underline;
}
.note-list .abstruct {
    margin-bottom:10px;
    font-size:13px;
    line-height:24px;
}
.note-list .meta {
    font-size:12px;
    font-weight: 400;
    line-height:20px;
}
.note-list .meta .origin-author {
    display: inline-block;
    margin-bottom: 5px;
    font-size: 12px;
    color: #969696;
}
.note-list .meta .origin-author a{
    color: #3194d0;
}
.note-list .meta a {
    color:#b4b4b4;
    transition: .1s ease-in;
    margin-right:10px;
}
.note-list .meta a:hover {
    color:#787878;
}
.note-list .meta span {
    color:#b4b4b4;
}
</style>
