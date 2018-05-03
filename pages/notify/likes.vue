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
                        <div class="menu">收到的喜欢和赞</div>
                        <ul class="like-list">

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
</style>
