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
               </div>
               <div class="col-xs-offset-1 col-xs-7 aside">
                   侧边栏
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
  data() {
    return {
      name: "首页"
    };
  }
};
</script>

<style scoped>

</style>
