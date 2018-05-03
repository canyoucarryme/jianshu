<template>
  <div class="aside">
                    <ul>
                        <li>
                            <nuxt-link to="/notify/comments">
                                <i class="fa fa-comment-o"></i>
                                    <span>评论</span>        
                            </nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/notify/chats">
                                <i class="fa fa-envelope-o"></i>
                                    <span>简信</span>        
                            </nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/notify/likes">
                                <i class="fa fa-heart-o"></i>
                                    <span>喜欢和赞</span>        
                            </nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/notify/follows">
                                <i class="fa fa-square-o"></i>
                                    <span>关注</span>        
                            </nuxt-link>
                        </li>
                    </ul>
    </div>
</template>

<script>
    export default {
        name:"myAside",
        data () {
            return {
                
            }
        }
    }
</script>

<style scoped>
    .aside{
        position: fixed;
        top: 0;
        bottom: 0;
        margin: 86px 0 0;
        padding: 0 0 30px;
        width: 280px;
        overflow: auto;
    }
    .aside ul{
        position: absolute;
        left: 0;
        min-width: 160px;
        z-index: 999 ;
        margin-bottom: 0;
        font-size: 15px;
        background-color: white;
        width: 100%;
    }
    .aside ul li a{
        height: auto;
        padding: 10px 25px;
        line-height: 30px;
        display: block;

    }
    .aside ul li a:hover{
        background: #f0f0f0;
    }
    .aside ul li a i{
        margin-right: 15px;
        font-size: 24px;
        color: #ea6f5a;
        vertical-align: middle;
    }
    .aside ul li a span{
        vertical-align: middle;
        font-size: 15px;
    }
</style>
