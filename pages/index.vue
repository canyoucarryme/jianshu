<template>
    <div style="height:100%">
        <my-header></my-header>
        <div class="container index">
           <div class="row">
               <div class="col-xs-16 main">
                   <!-- 热门专题 -->
                   <div class="recommend-collection">
                       <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c1.jpg">
                            <span class="name">故事</span>
                       </nuxt-link>
                       <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c1.jpg">
                            <span class="name">摄影</span>
                       </nuxt-link>
                       <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c2.jpg">
                            <span class="name">人文社科</span>
                       </nuxt-link>
                       <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c2.jpg">
                            <span class="name">历史</span>
                       </nuxt-link>
                       <nuxt-link class="collection" to="/collection/123">
                            <img src="~assets/img/c3.jpg">
                            <span class="name">读书</span>
                       </nuxt-link>
                       <nuxt-link class="more-collection" to="/collection/123">
                            更多热门专题
                            <span class="fa fa-angle-right"></span>
                       </nuxt-link>
                   </div>
                   <div class="splite-line"></div>
                   <!-- 文章列表 -->
                   <div class="list-container">
                       <ul class="note-list">
                           <li class="have-img">
                               <nuxt-link to="/p/123" class="wrap-img">
                                    <img  src="~/assets/img/note.png">
                               </nuxt-link>
                               <div class="content">
                                   <div class="author">
                                       <nuxt-link to="/p/123" class="avatar">
                                            <img src="~/assets/img/default-avatar.jpg">
                                       </nuxt-link>
                                       <div class="info">
                                           <nuxt-link to="/u/123" class="nickname">
                                            测试用户
                                           </nuxt-link>
                                           <span class="time">
                                               04.12 10:18
                                           </span>
                                       </div>
                                   </div>
                                   <nuxt-link class="title" to="/p/123">佛系程序员的月薪五万指南</nuxt-link>
                                   <div class="abstruct">
                                       摘要： 大师：很简单，我这里有一份佛系月薪 5 万指南，我看你骨骼清奇、脑门光亮，一看就是将要大富大贵之人，这份指南可以助你快速实现小目标！
                                   </div>
                                   <div class="meta">
                                       <nuxt-link to="/c/123" class="collection-tag">
                                            社会与法
                                       </nuxt-link>
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
                           <li>
                               <div class="content">
                                   <div class="author">
                                       <nuxt-link to="/p/123" class="avatar">
                                            <img src="~/assets/img/default-avatar.jpg">
                                       </nuxt-link>
                                       <div class="info">
                                           <nuxt-link to="/u/123" class="nickname">
                                            测试用户
                                           </nuxt-link>
                                           <span class="time">
                                               04.12 10:18
                                           </span>
                                       </div>
                                   </div>
                                   <nuxt-link class="title" to="/p/123">佛系程序员的月薪五万指南</nuxt-link>
                                   <div class="abstruct">
                                       摘要： 大师：很简单，我这里有一份佛系月薪 5 万指南，我看你骨骼清奇、脑门光亮，一看就是将要大富大贵之人，这份指南可以助你快速实现小目标！
                                   </div>
                                   <div class="meta">
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
                            <li class="have-img">
                                <nuxt-link to="/p/123" class="wrap-img">
                                    <img src="~/assets/img/note.png">
                                </nuxt-link>
                                <div class="content">
                                    <div class="author">
                                        <nuxt-link to="/p/123" class="avatar">
                                            <img src="~/assets/img/default-avatar.jpg">
                                        </nuxt-link>
                                        <div class="info">
                                            <nuxt-link to="/u/123" class="nickname">测试用户</nuxt-link>
                                            <span class="time">
                                                04.12 10:18
                                            </span>
                                        </div>
                                    </div>
                                    <nuxt-link class="title" to="/p/123">佛系程序员的月薪五万指南</nuxt-link>
                                    <div class="abstruct">
                                        摘要：大师：很简单，我这里有一份佛系月薪 5 万指南，我看你骨骼清奇、脑门光亮，一看就是将要大富大贵之人，这份指南可以助你快速实现小目标！ 程序员问大师…… 青年：大师，你看...
                                    </div>
                                    <div class="meta">
                                        <nuxt-link to="/c/123" class="collection-tag">社会与法</nuxt-link>
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
                            <li>
                                <div class="content">
                                    <div class="author">
                                        <nuxt-link to="/p/123" class="avatar">
                                            <img src="~/assets/img/default-avatar.jpg">
                                        </nuxt-link>
                                        <div class="info">
                                            <nuxt-link to="/u/123" class="nickname">测试用户</nuxt-link>
                                            <span class="time">
                                                04.12 10:18
                                            </span>
                                        </div>
                                    </div>
                                    <nuxt-link class="title" to="/p/123">佛系程序员的月薪五万指南</nuxt-link>
                                    <div class="abstruct">
                                        摘要：大师：很简单，我这里有一份佛系月薪 5 万指南，我看你骨骼清奇、脑门光亮，一看就是将要大富大贵之人，这份指南可以助你快速实现小目标！ 程序员问大师…… 青年：大师，你看...
                                    </div>
                                    <div class="meta">
                                        <nuxt-link to="/c/123" class="collection-tag">社会与法</nuxt-link>
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
                <a href="#" class="load-more">阅读更多</a>
               </div>
               <div class="col-xs-offset-1 col-xs-7 aside">
                  <div class="row">
                      <!-- 广告 -->
                    <div class="board">
                      <nuxt-link to="/">
                        <img src="~assets/img/ad1.png">
                      </nuxt-link>
                      <nuxt-link to="/">
                        <img src="~assets/img/ad2.png">
                      </nuxt-link>
                      <nuxt-link to="/">
                        <img src="~assets/img/ad3.png">
                      </nuxt-link>
                      <nuxt-link to="/">
                        <img src="~assets/img/ad4.png">
                      </nuxt-link>
                    </div>
                    <!-- 推荐作者 -->
                    <div class="recommended-author">
                        <div class="title">
                            <span>推荐作者</span>
                                 <transition>
                                    <nuxt-link to="/" class="page-change">
                                        <i class="fa fa-refresh"></i>
                                        换一批
                                    </nuxt-link>
                                 </transition>
                            <ul class="recommended-list">
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~/assets/img/default-avatar.jpg" >
                                    </nuxt-link>
                                    <a href="#" :class="[isFollow?'follow':'following']" @click="isFollow=!isFollow" @mouseover="isCancel=!isCancel" @mouseout="isCancel=!isCancel">
                                        <i :class="[isFollow?'fa fa-plus':isCancel?'fa fa-check':'fa fa-close']"></i>
                                        {{isFollow?"关注":isCancel?"已关注":"取消关注"}}
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了1958k字·1.9k喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~/assets/img/default-avatar.jpg" >
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了1958k字·1.9k喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~/assets/img/default-avatar.jpg" >
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了1958k字·1.9k喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~/assets/img/default-avatar.jpg" >
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了1958k字·1.9k喜欢</p>
                                </li>
                                <li>
                                    <nuxt-link class="avatar" to="/u/123">
                                        <img src="~/assets/img/default-avatar.jpg" >
                                    </nuxt-link>
                                    <a href="#" class="follow">
                                        <i class="fa fa-plus"></i>
                                        关注
                                    </a>
                                    <nuxt-link to="/u/123" class="name">
                                        简书用户
                                    </nuxt-link>
                                    <p>写了1958k字·1.9k喜欢</p>
                                </li>
                            </ul>
                            <nuxt-link to="/" class="find-more">
                                查看更多
                               <i class="fa fa-angle-right"></i>
                            </nuxt-link>
                        </div>
                    </div>
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
    title: "简书-创作你的创作",
    meta: [
      { charset: "utf-8" },
      { name: "keywords", content: "简书首页" },
      { name: "description", content: "简书首页" },
      { name: "author", content: "wwj" }
    ]
  },
  components: {
    myHeader
  },
  data (){
    return {
      name: "首页",
      isFollow:true,
      isCancel:false,
    }
  },

  
}
</script>

<style scoped>

</style>
